# PTC-API-Playground

Welcome to the PTC API Playground! In this repository, you will find:
0. [Preface](link)
1. [Getting Started Documentation](link)
2. [Interactive Examples - Connecting to the "Master Snippets Document" for Google Colab](link)
3. Using the Snippets library and beyond!

## 0. Preface
**WELCOME TO THE PTC PLAYGROUND!**

This is meant to be the landing page for connecting to the [PTCColab](https://github.com/PTC-Education/PTCColab) Library/Python Package. The PTC-API-Playground is a library of examples that use PTCColab.

PTCColab was built with the intention of being a springboard for app development that use the Onshape API with basic connections to the Thingworx API. PTCColab can be used in any Python3 REPL however, PTC-API-Playground has been designed to work seemlessly with Google Colab, the Google Hosted Jupyter Notebook environment. The examples/"master snippet library" can be referenced for any Python Notebook or script. Specific documentation for PTCColab can be found [here](https://github.com/PTC-Education/PTCColab#table-of-contents), however it's recommended to follow the getting started guide below! Happy Hacking.


--- 

## 1. Getting Started
The first step for getting started with PTC API Playground is deciding what type of connections you want to make! Depending on what you want to connect to, different types of information (usually API keys) are needed. This step can be done after looking through examples of connections and various usages of PTCColab, although it's definitely easier to get started if you have all of the external set-up parts ready before hand diving in.

- Do you want to connect to Onshape?
  - ==> Get Onshape API Keys [here](https://dev-portal.onshape.com/) and instructions [here](https://github.com/PTC-Education/PTCColab#onshape-api-keys)
  - ==> You might also want to create an Onshape document/model in the workspace your API keys are for and have the URL handy.  
- Do you want to connect to Thingworx?
  - ==> Get Thingworx API Keys [instructions here](https://support.ptc.com/help/thingworx_hc/thingworx_8_hc/en/index.html#page/ThingWorx/Help/Composer/Security/ApplicationKeys/ApplicationKeys.html)
  - When connecting to Thingworx, you will also want a Thing Instance that's within the same Project as your API keys. To connect to Thingworx through PTCColab/PTC-API-Playground the Thing Instance URL must be in this format: `https://<Thingworx-Workspace-Base-URL>.portal.ptc.io/Thingworx/Things/<Thing-Name>/Properties/`

--- 

## 2. Interactive Examples - Connecting to the "Master Snippets Document" (For Google Colab)

Now onto getting the library of examples! You can find the mast Snippets Document directly in this repo ("PTC API Snippets.ipynb"). However this "master snippets" library is most useful integrated directly into your Google Colab Environment.

[Snippets Gif](link)

1. Open a document in [Google Colab](https://colab.research.google.com/). 
2. In the toolbar at the top (left) of your Google Colab you can go into the Tools > Settings > Sites Menu
3. Copy the Master Snippets Library URL: `https://colab.research.google.com/drive/1JmLNhqhKkH44XGOhvhFgVxpsxOAfD8on?usp=sharing` into the "Custom Snippet notebook URL box".
4. Hit save!
5. You can now open the snippets library in the menu on the left with the angled brackets: "<>". This is where all of the default snippets and the snippets from the "master snippets library" are.
6. Add them to your document!

---

## 3. Using the Snippets Library
I accidentally explained how to use snippets in the section above.

Below are some tips when connecting to PTCColab using Snippets
Outline of Snippets:
- 0.0 is a README Type
- 1.X is all of the snippets that involve PTCColab (which include connections to Onshape (1.2-1.6) and a basic connection to Thingworx(1.7-1.9))
- 2.X is a direct connection to Onshape's [official Python Client](https://github.com/onshape-public/onshape-clients)
- 3.X are traditional API calls to the Thingworx API using Python's request library.


General Tips:
- To connect to PTCColab using Snippets 1.1 is required to import the PTCColab library
- 1.2 is required to connect to any Onshape connection with PTCColab.
- 1.7 is required to connect to any Thingworx connection with PTC Colab.
- For any function in PTC Colab, there is probably an optional parameter called "verbose" which will give you more information into the black box. (Although you can see the implementation directly in the PTCColab repository.)
- Happy hacking!

