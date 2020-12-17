# IVR
**Class5** :material-menu-right: **IVR**

An **Interactive Voice Response (IVR)** allows callers to dial in and selection an extension for a specific department or group within the company. These extensions are routed to different SIP addresses, PSTN numbers, internal extension numbers, other IVRs, conference bridges, groups, and Class 5 applications, based on the key they press. When you create an **IVR**, you specify a 1:1 mapping for all the possible keys on the keypad. 
    
## IVR Planning 
Complete the following prior to configuring the **IVR**
    
1. Plan out the keys and desired destinations
2. Create an audio file (.pcm or .wav format) that greets the customer and explains the keypad options and their destinations. Ex: "Press 1 to speak with a sales agent. Press 2 to speak with a technical support agent" and so on. 
3. Upload this audio file to the ConnexCS Control Panel under **Management** :material-menu-right: **File**.

## Create an IVR

1. Click the `+` icon (located at the top-right corner of the page).
2. Configure the **Name** for the IVR.
3. Select the **Customer** from drop-down list.
4. Enter the **Extension** that callers must call to start interacting with the IVR.
5. Select the **Audio File** from the drop-down list (such as the one created in first step above) which plays the greeting and explains the keypad options. 
6. Once these fields are completed, you will be able to edit each key- numbers 0 to 9, '\*' (asterisk) and '#' (hash) - and configure what happens when the caller presses it.
7. Click `Edit` next to each key- numbers 0 to 9, '\*' (asterisk) and '#' (hash) - to edit the Destination. (`Edit` is not available until all required fields above are completed.)
    
    *   **External** - PSTN numbers that are outside your Class 5 network.
    *   **Internal** - Use extension numbers, IVRs, conference bridges, and groups.
   