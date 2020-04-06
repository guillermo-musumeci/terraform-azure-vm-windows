# Terraform Azure Windows Virtual Machine

Deploy a Windows Virtual Machine in Azure using Terraform

Update the **sku** on this section of the **windows-vm-main.tf** file, to configure the version of Windows Server. OS variables ae located on the file **windows-vm-variables.tf**

```
source_image_reference {
  publisher = "MicrosoftWindowsServer"
  offer     = "WindowsServer"
  sku       = var.windows-2019-sku
  version   = "latest"
}
```
