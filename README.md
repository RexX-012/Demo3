# Demo 3 

## How to get SSH Key

Step 1: In terminal do, ssh-keygen -t ed25519 -C "your_github_email@example.com" </n>
Step 2: > Enter a file in which to save the key (/Users/YOU/.ssh/id_ALGORITHM): [Press enter]
Step 3: Enter passphrase (empty for no passphrase): [Type a passphrase] &        
        RE-Enter same passphrase again: [Type passphrase again]
Step 4: Key generated

### Be careful key and key.pub are different. Public Key (.pub) is the one we keep in github or anyother public place.

## How to add SSH key to ssh agent

Step 1: In terminal do, eval "$(ssh-agent -s)" (Agent pid appears)
Step 2: ssh-add -K ~/.ssh/id_ed25519 (for mac) & ssh -add ~/.ssh/id_ed25519 (for win)
Step 3: Enter any password if existing then, its done.

## To check Fingerprint or public key

ssh -add -

1. L: shows the full public key for each agent
2. l: Shows the fingerprint, key length, and comment for all loaded keys.