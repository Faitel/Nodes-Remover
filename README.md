# Nodes Remover HDA for Houdini Indie

Deletes nodes and networks from the current project file

![Screenshot 2024-06-15 131821](https://github.com/Faitel/Nodes-Remover/assets/10779163/0b025996-1e5d-4d4b-80b9-8fd6e58a4510)

A simple node that deletes selected nodes or networks and optionally checks the hip filename for the presence of the string to prevent the node from deleting networks in the wrong file.

You can leave the field empty if you want to skip the validation.

This node is particularly useful when you want to send a copy of your hip file to the cloud and clean it from unnecessary stages or nodes that require Python scripts or other package dependencies that your cloud service may not have.

## Parameters description:

HIP Name Contains:

    The string parameter validates the project name before deleting nodes. Leave empty to skip validation. 
    
Node #:

    The parameter contains a path to the node or network to remove.
    
Display Messages:

    Outputs validation status and removing statistics either to message box or console.
    
Output Messages to Console:

    If toggled, it outputs validation and statistic messages to the console and the message box if not.
    
Output Nodes to Console:

    If toggled, print the list of deleted or skipped nodes to the console; otherwise, don't print anything.
