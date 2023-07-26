# Introduction

This is a short repo containing my notes for the course [Zero To Hero](https://karpathy.ai/zero-to-hero.html) by Andrej Karpathy. 

I found it a bit difficult to refer back to content at times and thought I'd organise them in a series of notebooks and other files.

## Setup

You can run each of the notebooks by simply installing the required dependencies

```bash
pip3 install -r requirements.txt
```

I suggest using a virtual environment, which can be configured using

```bash
python3 -m venv <name of virtual environment>
```

You can then activate it with 

```bash
source <name of virtual environment>/bin/activate
```

Once you've done so, don't forget to add the virtual environment to your ipykernel by running the command 

```bash
python -m ipykernel install --user --name=<what you want to call your virtual env in jupyter notebook>
```

## Content

### Lesson 1

- [Lesson 1](./lesson1/Lesson 1.ipynb)
- [BinaryClassification](./lesson1/lesson_1.ipynb)

## Troubleshooting

If you encounter the following message

```bash
File /Library/Frameworks/Python.framework/Versions/3.10/lib/python3.10/subprocess.py:1842, in Popen._execute_child(self, args, executable, preexec_fn, close_fds, pass_fds, cwd, env, startupinfo, creationflags, shell, p2cread, p2cwrite, c2pread, c2pwrite, errread, errwrite, restore_signals, gid, gids, uid, umask, start_new_session)
   1840     if errno_num != 0:
   1841         err_msg = os.strerror(errno_num)
-> 1842     raise child_exception_type(errno_num, err_msg, err_filename)
   1843 raise child_exception_type(err_msg)

PermissionError: [Errno 13] Permission denied: PosixPath('dot')
```

Then you might need to install the `dot` package. On MacOS, that can be done by using the command 

```
brew install dot
```

