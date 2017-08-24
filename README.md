## submodule

## create submodule
`git submodule add https://github.com/github/swift-style-guide`

`git status`
```
On branch master

Initial commit

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   .gitmodules
	new file:   swift-style-guide
```

`cat .gitmodules`
```
[submodule "swift-style-guide"]
	path = swift-style-guide
	url = https://github.com/github/swift-style-guide
```

`diff --git a/swift-style-guide b/swift-style-guide`
```
diff --git a/swift-style-guide b/swift-style-guide
new file mode 160000
index 0000000..926d7ba
--- /dev/null
+++ b/swift-style-guide
@@ -0,0 +1 @@
+Subproject commit 926d7ba8503fb5efcd0a890356862e1c89df1f00
```
`git commit -am "initial commit submodule swift-style-guide`
`git push`


## clone project with submodule
`git clone git@github.com:2w3/learn_submodule.git`  
`ls learn_submodule/swift-style-guide`  
`swift-style-guide` 디렉토리는 비어있다.

`cd learn_submodule && git submodule init`
```
Submodule 'swift-style-guide' (https://github.com/github/swift-style-guide) registered for path 'swift-style-guide'
```

`git submodule update`
```
Cloning into '/Users/snow/Documents/workspace/learn_submodule/swift-style-guide'...
Submodule path 'swift-style-guide': checked out '926d7ba8503fb5efcd0a890356862e1c89df1f00'
```
`ls swift-style-guide`
```
CONTRIBUTING.md LICENSE         README.md
```

