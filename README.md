# Direct Marketing w/ Amazon SageMaker

## Companion slides

https://view.highspot.com/viewer/5e40bc6d8117172723b125c1

## Setup instructions

### Login to your AWS account

1. Navigate to your AWS Management console: https://console.aws.amazon.com/
1. Login with your credentials
1. Make sure you are in the **N. Virginia** region by looking at the top right corner of the screen. It should say _N. Virginia_.

### Create your notebook instance

1. In the top bar menu, navigate to **Services > Amazon SageMaker** to open the SageMaker console.
1. In the navigation menu on the left, click **Notebook instances** (under **Notebook**).
1. Click on the **Create notebook instance** button.
1. Fill the following fields:
   * Notebook instance name: type a name for your instance, e.g `aim302`.
   * Notebook instance type: select **ml.t3.medium**. No need for anything bigger :)
   * Elastic Inference: leave this as `none`.
   * IAM role: select **Create a new role**. In the dialog window, do the following:
     * Select **Any S3 bucket** (under **S3 buckets you specify**).
     * Click on the **Create role** button.
     * Root access: leave this as `Enable`.
     * Encryption key: leave this as `No Custom Encryption`.
   * Click on the **Git repositories** section to expand it and do the following:
     * Select **Clone a public Git repository** from the dropdown list.
     * In the **Git repository** field, enter: `https://github.com/mikeapted/aim302.git`
   * Leave all other fields as is.
1. Click on the **Create notebook instance** button. This will bring you back to the list of Notebook instances where you should see yours being created. Wait for your Notebook instance to become **In Service** which should take less than 5 minutes. You may have to refresh the page depending on your browser.

### Log into your notebook

1. Next to your **Notebook instance**, click on the link **Open JupyterLab**. This will open the JupyterLab page in your browser.
1. In the **JupyterLab** page, on the navigation section on the left of the screen, double-click on **aim302.ipynb**. This will open the IPython Notebook.
1. The reminder of the lab instructions are in the aim302 notebook. Have fun!
