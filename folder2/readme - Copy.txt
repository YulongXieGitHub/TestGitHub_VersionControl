# **************** 
# PART 1: This exercise is based on the Youtube video [https://www.youtube.com/watch?v=mYjZtU1-u9Y]
# **************** 

[git init]
[git rm --cached filename]
[git log]
[git commit -m 'message']
[git status]


# ---------------------------------------------------------------------------------------------
# After one changes this file by adding the following
# do  [git diff] with show the differences 
# but [git diff --cached] will not show any differences ebcause the modified file is not in the staging area yet
#
# However, if the modified file is placed into the staging area by [git add readme.txt]
# do  [git diff] will show no difference
# but [git diff --cached] will show the difference because the differnce in the file in the staging area
# ---------------------------------------------------------------------------------------------

If [git log] cannot fit the screen once, need to [shift Z Z] to bring back the prompt.

[git log --oneline]

[git commit -a -m 'message']  -a means to put things in staging area.

[git status -s] show the modification in shorthand


Git Bash:
	[git init <project>]
	[git add <file or .>]
	[git commit -m "msg"]
	[git status]
	[git log]
	[git diff]
	[git diff --cached]

# **************** 	
# PART II: GitHub
# **************** 

	Suggest use a professional user name
	Suggest to create proper email account, do not be short-sighted.
	Suggest to have a strong password
	
	SSH Key:
	If one uses Git Bash, one needs to set this SSH up manually
	If one uses the Windows Git Client, it will do it automatically when one log in the first time.
	
	RSA key is a public and private key.  The private key will be on your computer and you will add the public key to GitHub.
	
	Once this is done, GitHub will trust your computer to upload code.
	
	
	-------------------------------------------------------------------------------------------
	1. Creating SSH Key: one will be using RSA public/private cryptography
	2. Combining with HTTPS or SSH to connect (either work but GitHub prefers SSH)
	3. search to see if one has a SSH folder
	
	ssh -keygen -t rsa -C "YulongGitHub@gmail.com"
	enter passphrase: "Pasword"
	
	now one shold have ".ssh" folder which consists of "id_rsa" and "id_rsa.pb".
	
	open "id_ras.pub" and copy and paste it to the SSH in github webpage
	
	check to see if SSH key work or not:
	
	[ssh -T git@github.com]	
	-------------------------------------------------------------------------------------------
	
	
	The author uses INDIGO "eclipse"
