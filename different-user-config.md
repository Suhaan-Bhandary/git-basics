# Different user config in Same PC

We can define a special config for a particular directory.

1. Create a directory named `work-environment`(can be any name)

2. Go to the global .gitconfig file in the home directory and paste the below code

```bash
[includeIf "gitdir:~/Desktop/work-environment/"]
	path = ~/.gitconfig-work
```

The above code tells git that if we are in the above directory then we can use `~/.gitconfig-work` for the directory.

3. Create `~/.gitconfig-work` and now you can specify the things in it.
