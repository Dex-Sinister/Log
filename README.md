# Log
MUX code for automated logging of scenes.

To set it up, create the objects in the Logging Master Object and Logging Parent Object files, including filling out &DB_LOG for the Logging Master Object.

After that, the commands work based on creating 'logger objects'. These are Things which have been set with the logging parent, and are designed to be targeted with commands on the logging master.

The commands are like so:

+log/setup <thing>: Sets the parent to turn a thing into a logger object. These can be @named, @desced, and moved around as with normal objects.

+log/on <logger>: Sets a logger to begin recording the poses in its room. Thus, this only works if the logger has been dropped out of inventory.

+log/re <logger>=<number>: Shows the last <number> poses the logger has recorded. Can be used be anyone, and including during recording.

+log/off <logger>: Makes an active logger stop recording.

+log/show <logger>: Shows all poses a logger has recorded. Can only be used from inventory by the owner or staff.

+log/wipe <logger>: Clears all poses from a logger object. Can only be used by the owner or staff.

+log/return <logger>: Returns a dropped logger object to its owner.
