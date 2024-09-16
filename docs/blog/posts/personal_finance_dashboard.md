---
date: 2024-01-02 
categories:
  - Data Engineering
  - Personal Finance
draft: true
---

# Create a Personal Finance Dashboard

## Shopping ticket retrieval

In this example, we will use the E.Leclerc shopping app to retrieve all my shopping tickets. To export E.Leclerc tickets, I advise you to access the E.Leclerc mobile App>My ticket and billing>Open a ticket> Share > Add to your drive. You can store all your tickets in a single folder you can access from your computer as we will parse the pdf to extract the needed information.

!!!note
    Tickets will be in the format text as pdf. If your tickets are scans, you will need to use an OCR tool to be able to extract the data from the ticket. Although, you can check the dependencies installation: [camelot install deps](https://camelot-py.readthedocs.io/en/master/user/install-deps.html)

## Extract data from tickets

To extract informations from tickets, we will use a the package pip install camelot-py [camelot-py](https://camelot-py.readthedocs.io/en/master/user/advanced.html#visual-debugging)

you will need to download [ghostscript](https://ghostscript.com/releases/gsdnld.html)

!!!warning
  You may have an error with ghostscript even though you installed it correctly. Try to restart your computer, it may resolve the problem of path

[:octicons-eye-24: | Access your azure account](https://portal.azure.com/#home){:target="_blank" .md-button .md-button--primary }

<!-- more -->

![image](../../assets/images/azure_create_account_storage.png)


```
