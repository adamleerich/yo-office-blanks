

## Yeoman Office Generator

Install Yeoman 

    npm install -g yo generator-office


Turn off diagnostic and usage reporting

    npx office-addin-usage-data off


Run generator

    yo office






| `projectType`            | Display Name                                                      | 
|--------------------------|-------------------------------------------------------------------| 
| `taskpane`               | Office Add-in Task Pane project                                   | 
| `react`                  | Office Add-in Task Pane project using React framework             | 
| `excel-functions-shared` | Excel Custom Functions using a Shared Runtime                     | 
| `excel-functions`        | Excel Custom Functions using a JavaScript-only Runtime            | 
| `single-sign-on`         | Office Add-in Task Pane project supporting single sign-on         | 
| `unified-manifest`       | Outlook Add-in with unified manifest for Microsoft 365 (preview)  | 
| `manifest`               | Office Add-in project containing the manifest only                | 





https://github.com/OfficeDev/generator-office/blob/master/src/app/config/projectProperties.json



```
yo office --projectType taskpane --name "010-taskpane-excel-ts" --host excel --ts --skip-install
yo office --projectType react --name "020-react-excel-ts" --host excel --ts --skip-install
yo office --projectType excel-functions-shared --name "030-excel-functions-shared-excel-ts" --host excel --ts --skip-install
yo office --projectType excel-functions --name "040-excel-functions-excel-ts" --host excel --ts --skip-install
yo office --projectType single-sign-on --name "050-single-sign-on-excel-ts" --host excel --ts --skip-install
yo office --projectType unified-manifest --name "060-unified-manifest-excel-ts" --host excel --ts --skip-install
yo office --projectType manifest --name "070-manifest-excel-ts" --host excel --ts --skip-install

yo office --projectType taskpane --name "011-taskpane-excel-js" --host excel --js --skip-install
yo office --projectType react --name "021-react-excel-js" --host excel --js --skip-install
yo office --projectType excel-functions-shared --name "031-excel-functions-shared-excel-js" --host excel --js --skip-install
yo office --projectType excel-functions --name "041-excel-functions-excel-js" --host excel --js --skip-install
yo office --projectType single-sign-on --name "051-single-sign-on-excel-js" --host excel --js --skip-install
yo office --projectType unified-manifest --name "061-unified-manifest-excel-js" --host excel --js --skip-install
yo office --projectType manifest --name "071-manifest-excel-js" --host excel --js --skip-install

gdni 010-taskpane-excel-ts\manifest.xml 011-taskpane-excel-js\manifest.xml
gdni 010-taskpane-excel-ts\manifest.xml 020-react-excel-ts\manifest.xml
gdni 010-taskpane-excel-ts\manifest.xml 021-react-excel-js\manifest.xml
gdni 010-taskpane-excel-ts\manifest.xml 030-excel-functions-shared-excel-ts\manifest.xml
gdni 010-taskpane-excel-ts\manifest.xml 031-excel-functions-shared-excel-js\manifest.xml
gdni 010-taskpane-excel-ts\manifest.xml 040-excel-functions-excel-ts\manifest.xml
gdni 010-taskpane-excel-ts\manifest.xml 041-excel-functions-excel-js\manifest.xml
gdni 010-taskpane-excel-ts\manifest.xml 050-single-sign-on-excel-ts\manifest.xml
gdni 010-taskpane-excel-ts\manifest.xml 051-single-sign-on-excel-js\manifest.xml
gdni 010-taskpane-excel-ts\manifest.xml 060-unified-manifest-excel-ts\manifest.xml
gdni 010-taskpane-excel-ts\manifest.xml 061-unified-manifest-excel-js\manifest.xml
gdni 010-taskpane-excel-ts\manifest.xml 070-manifest-excel-ts\manifest.xml
gdni 010-taskpane-excel-ts\manifest.xml 071-manifest-excel-js\manifest.xml

```





