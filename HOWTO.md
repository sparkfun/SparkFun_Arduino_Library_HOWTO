# Setting Up a SparkFun Arduino Library Repo

## Creating a Repository

When creating a repository, the preferred method is to create an empty repository and then copy in desired resources from this *HowTo* repository as needed.


1) Create a new repository on GitHub with the desired name for the library, following the template *SparkFun_<product name>_Arduino_Library*. When creating the repository, select the option to create a README.md file and a MIT License file. This will create the initial files for the repository and set up the license for the repository.
2) Once the repository created, the first step is to create branch - specifically a **develop** branch. This branch is used to stage changes and updates to the library before they are merged into the main branch. All of the initial development is performed on the develop branch, and then a GitHub PR is used to support the initial code review of the repository.
3) Clone the repository to your local machine and switch to the **develop** branch.

> [!NOTE]
> The HowTo repo is not used as a GitHub template to create a new repository due to how GitHub displays an annoying banner on repository created from a template. 

## License

SparkFun Arduino Libraries by default are published using the MIT OpenSource License. To attribute the repository with this license do the following:

### Repository Licensing

- In the root of the repository, include the file ***LICENSE*** that contains the text of the MIT license
  - When creating the repository, you can specify a license type of MIT and this file is created by GitHub

### README.md

At the bottom of the README.md file, include the following text to indicate the license for the repository:

```
## License Information

This product is ***open source***!

This product is licensed using the [MIT Open Source License](https://opensource.org/license/mit)
```

### Source Code Attribution

For each source file created, include the following text at the comment header at the top of the file:

```cpp
/*
 * @date 2026
 * @copyright Copyright (c) 2026, SparkFun Electronics Inc. This project is released under the MIT License.
 *
 * SPDX-License-Identifier: MIT
 */

```

Change the date and copyright date value as needed.


## Splash Images

To brand the repository for a library, a "splash" image is created and is the first element of the README.md file. 

The Splash Image for this repository:

![SparkFun How To Arduino Library](docs/images/gh-banner-howto-demo.png  "SparkFun HowTo Arduino Library")


The image uses one of the template image files contained in the [docs/images](docs/images) folder. To create a specific image, perform the following steps.

1) Select the image template to use from HowTo - make a local copy of this file
2) Open this file in your desired image editing tool (i.e. Photoshop, Pixelmator, GIMP ...etc).
3) Add the name of the repository item on the left section of the image.
4) Add an image of the target product as well as a tile for the board in the white area of the image
5) Save the image and add it to the "docs/images" folder of the new repository.
6) Set this image name in the linked image at the top of your repo README.md file

### Social Image

Additionally, upload the image as the social image for the new repository. To do this, perform the following:

- Navigate to the Settings page for the new repository
- In the **General** Section, under the section **Social preview** select the ***EditUpload*** button and the presented upload file entry.
- Select the local copy of the Splash Image created for the repository

The file is uploaded and available for the repo.

> [!NOTE]
> The social image is used to create preview tiles on the SparkFun Documentation landing page located at docs.sparkfun.com

## README.md