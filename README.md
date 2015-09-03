# ansibox

Ansibox is an idea and project from Jesse Keating to utilize ansible to manage configuration of a local system similar to boxen.

## What does it do?
Right now it provides a bare minimum feature set.
* On OSX it will install homebrew
* On Fedora it will remove and install whatever RPMs you list in the answer file
* On all systems it will sync in your dotfiles git repo if you have one

## Using ansibox

### Pre-requisites
* Install ansible

### Usage
* Populate answers.yaml with what you want on your system based on the main bits ansibox covers
* Optionally, create an additional playbook for ansibox to run after its own
* Run ansibox
    ./ansibox [optional playbook]
