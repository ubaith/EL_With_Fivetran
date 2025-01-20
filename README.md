# EL_With_Fivetran

Connecting Google Analytics with Fivetran

Steps

1. Start Fivetran Connector Setup:

   Log in to your Fivetran account.
   Navigate to the "Connectors" page and click "+ Connector".
  Search for and select "Google Analytics 4".

2. Authorize Fivetran with Google:

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
