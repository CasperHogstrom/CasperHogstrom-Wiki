# Using Git as a team and how to avoid common issues

Git is a tool that you have locally on your computer. To use it in a collaborative way you need a code hosting platform(let's shorten it to codehp). The most widely used one is Github and this is also the one I use.
A code hosting platform such as Github allows a team to push and pull code from a remote repo. With a codehp members can monitor commits and see the changes made which can be very useful to se what commit might have caused a problem even if one member might not be contactable atm.



## Common remote issues
* ### Merge issues
Git and a codehp enables a team to work within the same repo easily. But it is not without issues, a common problem one might encounter are merge issues. Merge issues appear when one or more lines of code occupies the same space and you try to pull or push from the remote repo. To solve this by hand git pull the code and either remove one or both of the conflicting lines of code. If you need both of the conflicting lines of code just move one of them to a unoccupied space and then perform the merge. 

If you don't need one of the conflicting lines of code you can solves this in the command line. To do this type git checkout --ours/theirs "filename". Depending on of you type ours or theirs you keep either the file as it is or you change it with yours.

If you realize that you have made an error(not that you would of course) or for some reason have to cancel the merger git merge --abort will be your ally. The command aborts the current merge with your merge issue.

To avoid merge issues it is always easier for all members to work in different documents or in different areas of the code. This often also helps with efficiency since you cover a bigger area of your work.

* ### It works on my pc!
Something that you hear from time to time is "It works on my pc"(with an underlying tone of aggression and blame). It can depend on a lot of things but in my experience it often has to do with you not being up to date with packets or having an old versions of the repo. Always try to just eliminate the simple things before going hacking the mainframe for solutions.