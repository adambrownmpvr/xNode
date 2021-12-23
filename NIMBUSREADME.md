This file outlines the changes made to the BASE xNode asset.

### [12/23/2021] ADAM BROWN ###

# Added
- Node:
	- CopyDynamicPorts()
	- VerifyNamesOfNodes()

# Changes
- NodeGraph: 
	- Added support for copying of DyanmicPorts in Copy()
	- Removed "(Clone)" from names of copied ports
	- Added renaming nodes when adding to graph
- NodeGraphWindow:
	- Added call for VerifyNamesOfNodes() in window open
	- Added call for VerifyNamesOfNodes() on Node creation

### [12/15/2021] ADAM BROWN ###

# Changes
- NodeEditor: Moved DrawProperties outside of pre-processor for not using Odin inspector
- NodeEditor: Added bool for drawing properties the standard way until we can understand Odin inspectors better

### [12/14/2021] ADAM BROWN ###

# Changes
- NodeEditor: DrawProperties and DrawDynamicPorts both now have excludes exposed to derived editors.

### [12/10/2021] ADAM BROWN ###

# Changes
- NodeEditorWindow: Open method now uses graph name as the window name.

### [12/07/2021] ADAM BROWN ###

# Changes
- NodeEditor: Created two new virtual methods: DrawProperties, and DrawDynamicPorts. Created to better utilize the base editor for extension.