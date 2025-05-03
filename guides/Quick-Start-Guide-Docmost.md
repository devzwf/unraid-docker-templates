# Quick Start Guide to launch Docmost on Unraid

### Step by Step

-   Go to Apps to install Redis (I prefer to use this one as it's more customizable : **bitnami/redis:latest** published by **A75G**).
    - **Redis Port**: `6379` is set by default.
    - **ALLOW_EMPTY_PASSWORD**: `no`
    - **Password**: Generation a strong one but don't put any @ inside.
    - **Appdata**: `/mnt/user/appdata/redis`
-   Go to Apps to install PostgreSQL, you can choose the v17.<br>
    - **Port: PostgreSQL access port**: If not in use, leave it. Default is **5432**.
    - **Path: /var/lib/postgresql/data**: `/mnt/user/appdata/postgresql17`
    - **Variable: POSTGRES_PASSWORD**: Generation a strong one but don't put any @ inside.
    - **Variable: POSTGRES_USER**: `postgres` is set by default.
    - **Variable: POSTGRES_DB**: `postgres` is set by default.
    - Once PostgreSQL is running, open its console and type this to setup a password to the postgres user previously created :<br>
     `su - postgres`<br>
     `psql`<br>
     `ALTER USER postgres PASSWORD 'THE_FAMOUS_STRONG_DB_PASSWORD';`  (don't put any @ sign)<br>
-   Go to Apps to install Docmost.<br> 
    - **Storage**: `/mnt/apps/appdata/docmost/data`
    - **Application URL**: `Un.raid.local.ip` You can also choose the URL you will use in Nginx later.
    - **Application Secret**: Generate a 32 lenght password.
    - **Database URL**: `postgresql://postgres:THE_FAMOUS_STRONG_DB_PASSWORD@LOCAL_IP_UNRAID:5433/postgres?schema=public` If you have changed the POSTGRES_USER and POSTGRES_DB, update them here.
    - **Redis URL**: `redis://:RedisPassword@LOCAL_IP_UNRAID:6379`
    - **WebUI**: `3000` is set by default.
    - Once Docmost is running, edit the container, switch to Advanced Mode and change : <br> `WebUI: https://[IP]:[PORT:3000]` to `WebUI: http://[IP]:[PORT:3000]`
