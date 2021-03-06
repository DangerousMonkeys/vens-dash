# Vensim Dashboard Generator

This app allows to build a decent looking dashboard from a Vensim system dynamics model and to run it locally on browser.

## Requirements

Before running this application, the Vensim web folder needs to be published first. The Vensim web publishing feature is available only on  v8.1+. 

The app also requires node.js to run.

## Usage

Clone the repository on your machine. Inside the repository there is a "sd" directory: replace that with your own directory, which is the one containing the system-dynamics model you want to publish (or a copy of it). Make sure the web folder within that has been published.

To launch the app: open the command line or terminal, change directory to the vensim-dash repo cloned on your machine and finally launch run.js via node:

```bash
cd "your\path\to\vens-dash\folder"
node run.js
```

Once the app is launched, the user can customize the dashboard view. If you change the model in the meantime, the view is still saved: republish the Vensim web folder and and relaunch the the run.js command. To go back to the default view, clear the /public/config/ folder.

## Limitations

Being built on top of the Vensim Web folder, this app has same limitation as for the models complexity it can support. It supports all functiona and subscript, but not read from file or optimization for example. For the same reason, the graphs that can be visualized as of now are just one-variable line graphs, not bar charts or stack graphs for example.

## Next steps
The Vensim Dashboard generator is still work in progress. Next steps for development:
* capability to add charts
* capability to remove sliders and charts and diagrams
* capability to add more than one dashboard view
* capability to load diagrams
* capability to customize landing, intro and links page
* capability to compare variables in the graph (for a singular scenario)
* capability to use different visualizations than just line charts
