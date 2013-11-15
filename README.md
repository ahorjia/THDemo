# Introduction
The introduction of FP Haskell Center(TM) community edition means that sharing your projects
with others is now easier than it has ever been before. Doing so means they can edit, test and
contribute to your project without having to install any software on their system or download
and unpack your project. They can start testing, editing and contributing with a single click.

This project will show you how.

# Sharing from FP Haskell Center

## Publish
First, you need to publish your article. Click the `Publish` icon in the menu bar. It is a curved
arrow pointing out of the page.

This will bring up a commit pane. Add a comment relevant to what's being published, and then
commit it. You will need to do this even if their are no changes from the current head in your
workspace. It will work like [this link](https://www.fpcomplete.com/school/using-fphc/sharing-projects-with-fp-haskell-center).

## Share
You are done. You can share the URL of your project with others just as it is - post it to reddit,
facebook, or LinkedIn
in your announcement of the project, link to it in a StackOverflow question about the code, letting
people easily try their solutions before answering your question.

# Sharing a git repository
If your project is in a git repository that can be reached from the internet, you can share it in
with FP Haskell Center. A link of the form `https://www.fpcomplete.com/ide?git=*git-url*` will clone the
git repository in the community edition, and then open that project.

This works well with [github](https://github.net/). For instance, to clone a popular Yesod example, use the url 

[http://www.fpcomplete.com/ide?git=https://github.com/snoyberg/yesod-web-service-tutorial.git](http://www.fpcomplete.com/ide?git=https://github.com/snoyberg/yesod-web-service-tutorial.git).


# Sharing from lpaste.net
If your project is in an [lpaste.net](http://lpaste.net/) pastie, it will have an `Open in IDE` button
in the menu bar. If a user clicks that, it will clone the code into a new FP Haskell Center project.

By default, your code will be put in `Main.hs` in the project. You can set the file name by starting the
pastie with a comment like: `{-# START_FILE *MyFile.hs* #-}`.
This will cause the following content to go into `MyFile.hs`. If you use the `START_FILE` comment more than
once, each occurence will cause the following content to go into different files - with the names you
provided - when the pastie is cloned.

# Sharing from anywhere
If you have a web site where you can export your project as a plain text file, you can share it in
the FP Haskell Center. Putting it on [DropBox](https://www.dropbox.com/), for instance.

In order to clone a project from anywhere, you use a URL of the form
`https://www.fpcomplete.com/ide?title=*Title*&paste=*content-url*`. The `Title` will be used for the title
of your project. The `content-url` will be fetched to get the files for the project. That should return
plain text.

By default, the fetched text will be put in `Main.hs` in the project. You can set the file name by starting the
pastie with a comment like: `{-# START_FILE *MyFile.hs* #-}`.
This will cause the following content to go into `MyFile.hs`. If you use the `START_FILE` comment more than
once, each occurence will cause the following content to go into different files - with the names you
provided - when the pastie is cloned.

Here's a [simple example](https://www.fpcomplete.com/ide?title=3+Bobs&paste=https://dl.dropboxusercontent.com/u/41598573/3bobs.hs).
