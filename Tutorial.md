# Setting up your Extension Development Environment

The purpose of this tutorial is to guide you through setting up your computer environment so that you can write and publish NVIDIA Omniverse extensions. You will take the following steps:

- [1. Install Software](#1-install-software)

    -[1.1 Omniverse](#11-omniverse)

    -[1.2 Omniverse Code](#12-omniverse-code)

    -[1.3 VS Code](#13-vs-code)

    -[1.4 GIT](#14-git)

- [2. Create a GitHub Account](#2-create-a-github-account)

- [3. Create a New Extension](#3-create-a-new-extension)

    -[3.1 Launch Code](#31-launch-code)

    -[3.2 Set Your Project Path](#32-set-your-project-path)

    -[3.3 Create the Extension](#33-create-the-extension)

    -[3.4 Extension Learning Resources](#34-extension-learning-resources)

- [4. Create a GIT Repository](#4-create-a-git-repository)

    -[4.1 Create the repository](#41-create-the-repository)

    -[4.2 Publish the Repository to GitHub](#42-publish-the-repository-to-github)

    -[4.3 Choose a Public or Private Repository](#43-choose-a-public-or-private-repository)

    -[4.4 Open the Repository on GitHub](#44-open-the-repository-on-github)

- [5. Release Your Extension to the Omniverse Community](#5-release-your-extension-to-the-omniverse-community)

    -[5.1 Add the `omniverse-kit-extension` Topic](#51-add-the-omniverse-kit-extension-topic)

    -[5.2 Create a Release](#52-create-a-release)

    -[5.3 Make the Repository Public](#53-make-the-repository-public)

- [6. Conclusion](#6-conclusion)

Check out this video if you only need the GIT portions of this tutorial:

<p align="center">
    <a href="https://www.youtube.com/watch?v=lEQ2VmzXMgQ">
        <img src="https://img.youtube.com/vi/lEQ2VmzXMgQ/0.jpg" width=50%>
    </a>
<p>

## 1 Install Software

### 1.1 Omniverse

You can find Omniverse [here](https://www.nvidia.com/en-us/omniverse/). To download it click on the green `Get Started` button and then click on the green `download` button for an invdividual user.

Once downloaded you can follow the installation instructions found in the video below to complete your installation and optionally set up a nucleus server:

<p align="center">
    <a href="https://www.youtube.com/watch?v=MbsFBukGOZE">
        <img src="https://img.youtube.com/vi/MbsFBukGOZE/0.jpg" width=50%>
    </a>
<p>

### 1.2 Omniverse Code

Open Omniverse launcher that you just installed. Navigate to the `Exchange` tab at the top. Enter `Code` into the search bar and click on the `Omniverse Code` app. Click on the green `Install` button in the upper right hand corner. The installation will proceed automatically from this point.

### 1.3 VS Code

You can find VS code [here](https://code.visualstudio.com/). To download it click on the blue `Download` button. Once downloaded perform the standard installation.

<p align="center">
    <a href="https://code.visualstudio.com/">
        <img src="Images/VSCode.png" width=50%>
    </a>
<p>

### 1.4 GIT

You can find the GIT downloads [here](https://git-scm.com/downloads). Click on the button for your operating system such as Windows or macOS. There are various options as you complete this download but the default options have worked well for me in the past.

<p align="center">
    <a href="https://git-scm.com/downloads">
        <img src="Images/GITDownloads.png" width=50%>
    </a>
<p>

## 2. Create a GitHub Account

If you don't have a GitHub account already, the next step is to create one. You create your account at the GitHub home page [here](https://github.com/). Once at the GitHub home page click on the `Sign Up` button in the upper right and follow their instructions. 

<p align="center">
    <a href="https://github.com/">
        <img src="Images/GitHubHome.png" width=50%>
    </a>
<p>

## 3. Create a New Extension

In this section you will create a new extension inside NVIDIA Omniverse

### 3.1 Launch Code

To create a new extension, open the omniverse launcher. Next navigate to the `Library` tab. Click on the `Code` item on the left and then click the white `Launch` button.

### 3.2 Set Your Project Path

At this point it is a good idea to make sure you have a standard folder on your computer where you will put all of your GIT repositories. On my windows computer I like this to be at `C:/Users/YOUR_USER_NAME/Repos`. If you don't already have a folder where you store your code, go ahead and create that now.

### 3.3 Create the Extension

Once the Code application opens, click on the `Extensions` tab. Click on the green `+` button and then `New Extension Template Project`. Select your `Repos` folder and click `Create`. Choose a name for the folder your project will be stored in and click `Ok`.

Next you need to name your extension. The first part of the name should be your personal namespace. You can choose any namespace unique to you. After that are one or two `.` delimited words that describe your extension. The first word should be more general and if you have a second word it should be more specific. For example, if I wrote an excel reading sample I would name it `UniqueNamespace.Sample.Excel`.

Click ok and Omniverse will create your extension and launch visual studio code to your extension's folder.

### 3.4 Extension Learning Resources

At this point you will write your extension. I highly recommend the tutorials [here](https://developer.nvidia.com/nvidia-omniverse-developer-resource-center#extn_creating) and that you join us on [Discord](https://discord.gg/BnEFJvcG) where you can chat with community members, NVIDIA developers, and participate in frequent Omniverse hangouts and hackathons.

## 4. Create a GIT Repository

In this section you will create a GIT repository containing your extension and publish it to GitHub.

### 4.1 Create the Repository

To create a GIT repository navigate to the `Source Control` tab in visual studio code.

<p align="center">
        <img src="Images/VSCodeTabs.png" width=5%>
<p>

### 4.2 Publish the Repository to GitHub

Next click on the blue `Publish to GitHub`. If this is your first time connecting to GitHub from Visual Studio Code you will have to click `allow` when prompted and complete the GitHub login prompt to authorize Visual Studio to access GitHub.

<p align="center">
        <img src="Images/PublishToGitHub.png" width=30%>
<p>

### 4.3 Choose a Public or Private Repository

Once you do this, two options will appear in a text entry at the top of Visual Studio. One is the option to publish a private repository to GitHub and one is to publish a public repository. I recomend you select a private repository for now and change it to a public repository when you are ready to share your extension with the world.

<p align="center">
        <img src="Images/PublishToPrivate.png" width=50%>
<p>

### 4.4 Open the Repository on GitHub

If this is your first time publishing to GitHub you may be prompted to sign into github in your browser. There may also be a few popups in the lower right of Visual Studio. I usually select `Open in Github` if prompted and I usually select to periodically fetch to keep my local repo up to date if I am collaborating with others. Using GIT is a topic in itself, but to get started you can write your code, go do the `Source Control` Tab, write a message in the `Commit Message` box, click the check mark to commit your code, and hit the sync button to sync your code with the GitHub server.

## 5. Release Your Extension to the Omniverse Community

In order for your extension to show up directly in the omniverse extensions window, you have to do three things.

1. Add the `omniverse-kit-extension` topic to your repo
2. Create a release
3. Make your repo public

All three of these things are done from your repository on the GitHub website, so first go to GitHub and from your home page select your extension's repository.

### 5.1 Add the `omniverse-kit-extension` Topic

Once in your repository, click on the gear in the `About` section of your repo.

<p align="center">
        <img src="Images/GitHubAbout.png" width=70%>
<p>

In the popup that appears, add `omniverse-kit-extension` to the topics text field.

<p align="center">
        <img src="Images/GitHubTopic.png" width=40%>
<p>

Click `Save changes`.

### 5.2 Create a Release

To create a release click on the `Create a new release` link in the `Releases` section on the right hand side.

<p align="center">
        <img src="Images/GitHubCreateNewRelease.png" width=70%>
<p>

Once your are on the release page you need to:

1. Click on `Choose a tag`
2. Enter a name such as `v1.0` for your tag
3. Click on `+ Create a new tag`
4. Click on `Publish release`

<p align="center">
        <img src="Images/GitHubFinalizeRelease.png" width=70%>
<p>

### 5.3 Make the Repository Public

When your extension is complete and you are ready for it to appear in the extension catalog within Omniverse, go to your repository settings, scroll down to the `Danger Zone` and make your repository public.

## 6. Conclusion

In this tutorial you learned how to Install the software you need to create Omniverse extensions, create a GitHub account, create an extension, publish an extension to GitHub, and make the extension available to the community within Omniverse.  

To learn more about extension building be sure to check out our #ExtendOmniverse at [CONTEST LINK TO COME] and find more resources [here](https://developer.nvidia.com/nvidia-omniverse-developer-resource-center#extensions)
