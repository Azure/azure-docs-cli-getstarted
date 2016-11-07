---
title: Get started with Azure 2.0 CLI Preview 
description: Get started with Azure 2.0 CLI Preview on Linux, Mac, or Windows.
keywords: Azure CLI 2.0, Linux, Mac, Windows, OS X, Ubuntu, Debian, CentOS, RHEL, SUSE, CoreOS, Docker, Windows, Python, PIP
author: allclark
manager: douge
ms.date: 11/01/2016
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.assetid: 85c418a8-6177-4833-bb8d-ff4ce2233c1a
---

# Get started with Azure 2.0 CLI Preview

1. [Install Azure CLI 2.0 Preview](https://github.com/Azure/azure-cli/blob/master/doc/preview_install_guide.md)
on whatever platform you use.

2. Run the `az` command to verify the installation.

3. Log in to your Azure account.

    ```azurecli
    az login
    ```

    You'll be prompted to open https://aka.ms/devicelogin and enter a code.

    ```azurecli
    To sign in, use a web browser to open the page https://aka.ms/devicelogin. Enter the code ******** to authenticate.
    ```

    You'll be prompted to log in using your credentials.
    
Now you can run any command that accesses your account.

Here are some other things to try:

- Create a resource group

    ```azurecli
    az resource group create -l westus -n MyRG
    ```

- Create a VM

    ```azurecli
    az vm create -g MyRG -n MyVM --admin-username admin --admin-password Password@1234
    ```

- Look at more [samples](https://github.com/Azure/azure-cli-samples).

- Get help.

    ```azurecli
    az [command-group [command]] -h
    ```

    For example, to get see what commands and subgroups are available for VMs, use

    ```azurecli
    az vm -h
    ```

    To get help with the command to create a VM, use

    ```azurecli
    az vm create -h
    ```

- Read the [API reference docs](../index.md).

- Send us your feedback using `az feedback`.