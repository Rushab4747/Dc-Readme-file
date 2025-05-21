# Manual Configuration of Environment Variables in Azure Function App
This guide explains how to manually configure environment variables in your Azure Function App after deploying your function code. If your code references specific environment variables (e.g., for accessing a storage account), these must be manually defined within the Function App settings.

## Prerequisite
Ensure your Function App is already created and the function code is deployed.

## Why This is Needed?
If your function code uses environment variables—like connection strings, API keys, or storage credentials—you need to define them within the Azure Function App environment for your code to work properly.

##  Steps to Configure Environment Variables
### 🔹 Step 1: Open Your Function App in Azure
Navigate to your Azure portal and go to the Function App you have deployed. In the left-hand panel, use the search bar and search for “Environment Variables”.

[![Step 1 - Open Function App](images/functionapp1.png)](images/functionapp1.png)


---

### Step 2: Add a New Environment Variable
Click the `+ Add` button to begin adding a new environment variable.

[![Step 2 - Add Environment Variable](image/functionapp2.png)](image/functionapp2.png)

---

### Step 3: Provide Name and Value
In the dialog that appears:

- Name: Enter the variable name as used in your code.
- Value: Provide the corresponding value.
Click OK and Save after adding each variable.

[![Step 3 - Provide Name and Value](image/functionapp3.png)](image/functionapp3.png)

---

## ✅ Example

If your code has something like:

python
storage_account = os.environ['STORAGE_ACCOUNT_KEY']


Things to Remember
All environment variables must exactly match the names used in the code.
Secrets should never be hardcoded in your code—they should always be placed in environment variables or secured with Azure Key Vault.
