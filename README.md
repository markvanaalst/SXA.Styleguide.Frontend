 ![Image alt text](/docs/img/styleguide.png)

The SXA Styleguide is an education site based on SXA that helps explaining the inner working and illustrating best practices. 

This repository holds all the frontend code needed to run the site. It consists of two parts, the SXA themes and the Scriban templates used on the site. The folder structure used in this repository mimics the SXA Creative Exchange output, therefore you can find the sources for the themes and the seperate scriban templates in the following folders:
|Type|Location
-|-
Theme|\src\-\media\Themes\Sitecore\Styleguide\Styleguide\
Extension Theme|\src\-\media\Extension Themes\CSS Animations
Scriban|src\-\scriban

### Requirements
The Styleguide is built to support **[Sitecore Experience Platform 9.3](https://dev.sitecore.net/Downloads/Sitecore_Experience_Platform/93/Sitecore_Experience_Platform_93_Initial_Release.aspx)** using **[Sitecore Experience Accelerator (SXA) 9.3](https://dev.sitecore.net/Downloads/Sitecore_Experience_Accelerator/9x/Sitecore_Experience_Accelerator_930.aspx)**.

### Prerequisites
   
*If you have already configured Creative Exchange you can skip the first step*

1. Open *PathToSitecoreInstance/Website/App_Config/Include/z.Feature.Overrides* folder and remove **.disabled** from **z.SPE.Sync.Enabler.Gulp.config.disabled** file;
2. Clone the repository
3. Switch to this repository and open `\src\-\media\Themes\Sitecore\Styleguide\Styleguide\gulp\config.js`
4. Update config file for Gulp tasks:
    `serverOptions.server` - path to sitecore instance. Example `server: 'http://www.sxa.sc'`;

5. go to the folder `\src\-\media\Themes\Sitecore\Styleguide\Styleguide\` using the command prompt (or VS Code terminal) 
6. Run `npm install` (*node.js and npm should be already installed*);
7. Run the gulp task to start Creative Exchange Live

*For detailed instructions on how to setup Creative Exchange Live please read the [readme](/src/-/media/Themes/Sitecore/Styleguide/Styleguide/readme.md) file*

### Visual Studio Code

In the repository there is a [Visual Studio code workspace](SXA.Styleguide.Frontend.code-workspace) that directly adds the folder locations mentioned previously.

Recommended VS Code extensions:
- [Scriban Syntax Coloring extension for Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=xoofx.scriban) - 
- [Sitecore Experience Accelerator Scriban syntax coloring and auto completion](https://marketplace.visualstudio.com/items?itemName=adamnaj.sitecore-scriban)

More information and documention on Scriban can be found at the [authors website](https://github.com/lunet-io/scriban)
Sitecore extensions to Scriban are documented on the official [Sitecore Documentation website](https://doc.sitecore.com/developers/sxa/93/sitecore-experience-accelerator/en/scriban-templates.html)


#### Disclaimer
The code, samples and/or solutions provided in this repository are unsupported by Sitecore Support. Support is provided on a best-effort basis via GitHub issues.

It is assumed that you already have a working instance of Sitecore XM and all prerequisites prior to installing this site. Support for product installation issues should be directed to relevant Community channels or through regular Sitecore support channels.

#### Warranty
The code, samples and/or solutions provided in this repository are for example purposes only and without warranty (expressed or implied). The code has not been extensively tested and is not guaranteed to be bug free.