# cst8919lab1

## Setup

### Step 1: Create an Auth0 Account/Application

1. Go to [Auth0](https://auth0.com/) and sign in, if a sign in has not be created, create one so you have accesses to the following settings.
2. Create a new **application**:
   - Type: **Regular Web Application**
   - Name: `Flask Login App` (or similar)
3. Under **Settings**, note the following:
   - `Domain`
   - `Client ID`
   - `Client Secret`
4. Set Allowed URLs:
   - **Allowed Callback URLs**: `http://localhost:3000/callback`
   - **Allowed Logout URLs**: `http://localhost:3000`

------

### Step 2: Start venv and install dependencies

1. setup venv

   ```
   python3 -m venv venv
   ```

2. start venv

   ```
   source venv/bin/activate
   ```

3. exit venv

   ```
   deactivate
   ```

Install dependencies in venv:

```
pip install -r requirements.txt
```

The Rquirement text file should contain the following:

```
flask>=2.0.3
python-dotenv>=0.19.2
authlib>=1.0
requests>=2.27.1
```

------

## **3. Environment Variables**

Create a `.env` file:

```
AUTH0_CLIENT_ID=
AUTH0_CLIENT_SECRET=
AUTH0_DOMAIN=
APP_SECRET_KEY=
```

Generate the string for `APP_SECRET_KEY` by using `openssl rand -hex 32` from the terimal.

------

## **4. Flask Logic**

Follow the Auth0 Flask Quickstart and implement login/logout routes for the application and label the file server.py.

## **5. Run the application**

Once the Quickstart has been completed, run the following command to see the results.

```
python3 server.py
```
or 
```
python server.py
```

## **Demo Video **
Link:
