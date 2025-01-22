# EL_With_Fivetran

## Connecting Google Analytics with Fivetran

Steps

1. Start Fivetran Connector Setup:

   Log in to your Fivetran account.

   Navigate to the "Connectors" page and click "+ Connector".

   Search for and select "Google Analytics 4".

3. Authorize Fivetran with Google:

  In the connector setup form, provide a destination schema name (this is the name of the schema in your data warehouse where the data will be loaded).
  
  Click "Authorize with Google" and log in to your Google Analytics account.
  
  Grant Fivetran the necessary permissions to access your Google Analytics data.

3. Configure Sync Options:

  Historical Sync Time Frame: Choose how much historical data you want to initially sync.
  
  Accounts Sync Mode:
    
    Sync All Accounts: Syncs all accounts you have access to.
    
    Sync Specific Accounts: Allows you to select specific accounts and properties to sync. This is generally recommended for better control.
  
  (Optional) Add Custom Reports: If you need specific combinations of dimensions and metrics not included in Fivetran's pre-built reports, you can create custom reports.

4. Complete Setup and Initial Sync:

  Review your settings and click "Save & Test".
  
  Fivetran will begin the initial sync, which may take some time depending on the amount of data.


## Connecting Snowflake with Fivetran

1. Create a Destination Configuration in Fivetran:

   Log in to your Fivetran dashboard

   Click on the Add Destination button

   Name your destination and choose Snowflake as the destination type
   
2. Gather Snowflake Connection Details:

   You'll need the following information from your Snowflake account:

      Account Identifier: This is the unique identifier for your Snowflake account. It usually follows a format like xy12345.us-east-1 or xy12345.snowflakecomputing.com.

      User: A Snowflake user with appropriate privileges to write data.

      Password: The password for the specified user.

      Warehouse: The virtual warehouse in Snowflake that Fivetran will use for loading data.

      Database: The database in Snowflake where Fivetran will create schemas and tables.

3. Configure the Connection in Fivetran:

   In the Fivetran setup form, enter the Snowflake connection details you gathered in the previous step

   You can also specify a schema prefix to organize the schemas created by Fivetran in your Snowflake database

4. Test the Connection:

   Fivetran will test the connection to ensure it can successfully connect to your Snowflake account

5. (Optional) Configure Security:

     For enhanced security, you can configure network policies in Snowflake to restrict access to Fivetran's IP addresses.
