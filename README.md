# Demo 3 

## How to get SSH Key

Step 1: In terminal do, ssh-keygen -t ed25519 -C "your_github_email@example.com" <br>
Step 2: > Enter a file in which to save the key (/Users/YOU/.ssh/id_ALGORITHM): [Press enter]<br>
Step 3: Enter passphrase (empty for no passphrase): [Type a passphrase] &  <br>      
        RE-Enter same passphrase again: [Type passphrase again]<br>
Step 4: Key generated <br>

### Be careful key and key.pub are different. Public Key (.pub) is the one we keep in github or anyother public place.
<br>
## How to add SSH key to ssh agent<br>

Step 1: In terminal do, eval "$(ssh-agent -s)" (Agent pid appears)<br>
Step 2: ssh-add -K ~/.ssh/id_ed25519 (for mac) & ssh -add ~/.ssh/id_ed25519 (for win)<br>
Step 3: Enter any password if existing then, its done.<br>

## To check Fingerprint or public key
<br>
ssh -add -
<br>
1. L: shows the full public key for each agent.<br>
2. l: Shows the fingerprint, key length, and comment for all loaded keys.