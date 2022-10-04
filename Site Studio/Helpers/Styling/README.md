# Helpers&nbsp;&nbsp;/&nbsp;&nbsp;Styling

<p>&nbsp;</p>

[Acquia Site Studio](https://www.acquia.com/products/drupal-cloud/site-studio) must be installed for these configurations to operate.<br>
A helper catagory named **'Styling'** must exist within the **[Helper categories](https://sitestudiodocs.acquia.com/6.9/user-guide/component-form-helpers)** area of **Site Studio**.

<p>&nbsp;</p>

### Usage:

### Step 1 - Import the Helper category

- Navigate to **Configuration** in the Drupal administrator toolbar.
- Go to **Development > Configuration synchronization**. Then to the **Import** tab and select **Single item**.
- Under the **Configuration type** dropdown, select **Helper category**.
- Copy and paste the code content of the `cohesion_helper_category_(hlp_cat_styling)_styling.package` YML file into the **Paste your configuration here** field.
- Click **Import** and follow the instructions for syncing.
- To check if a configuration was properly imported navigate to **Site Studio** in the Drupal administrator toolbar.
- Go to **Helpers > Categories**, the imported configuration should be listed.

<p>&nbsp;</p>

### Step 2 - Import the individual form helpers

- Navigate to **Configuration** in the Drupal administrator toolbar.
- Go to **Development > Configuration synchronization**. Then to the **Import** tab and select **Single item**.
- Under the **Configuration type** dropdown, select **Helper**.
- Copy and paste the code content of an individual YML file into the **Paste your configuration here** field.
- Click **Import** and follow the instructions for syncing.
- To check if a configuration was properly imported navigate to **Site Studio** in the Drupal administrator toolbar.
- Go to **Helpers > Helpers**, the imported configurations should be listed under **Styling**.
