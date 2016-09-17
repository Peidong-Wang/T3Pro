# T3Pro
T3Pro: A Command Line Tool Notifying the User When A Program Finishes Using Twitter Direct Message

T3Pro is based on oysttyer. The idea is to use a child Twitter account to send direct message to the parent (main) account. If the parent account allows notifications sent by the child account, such a system can be used as a tool reminding the user when a program finishes. oysttyer is used to control the child account. Notifications will be received in the parent (main) account.

## Install

1. Create a new Twitter account (child account). Let the parent accound and the child account follow each other.
2. Configure oysttyer on the child account following the instructions on [http://oysttyer.github.io/docs/userGuide.html#apikey](http://oysttyer.github.io/docs/userGuide.html#apikey). An exeption is in the 3rd step. I suggest the Name to be "T3Pro (YourCoolTwitterHandle)", Description to be "A Command Line Tool Notifying the User When A Program Finishes Using Twitter Direct Message" and Website to be "https://github.com/pozhijisi/T3Pro".
3. Add RECEIVER in t3pro script. (This is the parent (main) account. For example my Twitter identifier is @wang_7642, I need to add wang_7642 here.)
4. `chmod u+x t3pro` (Grant execution privilege to t3pro. "u" means only you can execute T3Pro. "+x" means granting execution privilege.)
5. Add the path of t3pro to ~/.bash_profile or ~/.profile, according to your platform.
6. `source ~/.bash_profile` or `source ~/.profile`.

## Test

You may use `t3pro expr 1 + 1` to test whether T3Pro is successfully installed.

## Usage

`t3pro <your command>`

## Uninstall

T3Pro adds configuration files entirely in your own home directory. In another word, T3Pro is a local application.

There is nothing modified by T3Pro itself. All modifications are made by oysttyer.

For uninstallation, you may simply `rm ~/.oysttyerkey` and `rm ~/.oysttyerrc` (if you set up this configuration file, which is highly recommended).

After deleting the configuration files, you may simply delete the source code folder of T3Pro.

## To Do

1. Add a configure file.
2. Add uninstallation features.

## License

oysttyer uses Floodgap Free Software License.

I further restrict T3Pro to be under GNU 3 License.
