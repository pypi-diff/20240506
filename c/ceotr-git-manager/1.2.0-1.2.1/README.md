# Comparing `tmp/ceotr_git_manager-1.2.0.tar.gz` & `tmp/ceotr_git_manager-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ceotr_git_manager-1.2.0.tar", last modified: Tue Mar 12 18:47:29 2024, max compression
+gzip compressed data, was "ceotr_git_manager-1.2.1.tar", last modified: Mon May  6 05:42:47 2024, max compression
```

## Comparing `ceotr_git_manager-1.2.0.tar` & `ceotr_git_manager-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxr-x   0 elliskeener-lacroix  (1000) elliskeener-lacroix  (1000)        0 2024-03-12 18:47:29.400017 ceotr_git_manager-1.2.0/
--rw-rw-r--   0 elliskeener-lacroix  (1000) elliskeener-lacroix  (1000)      162 2024-03-06 16:42:33.000000 ceotr_git_manager-1.2.0/LICENSE.md
--rw-r--r--   0 elliskeener-lacroix  (1000) elliskeener-lacroix  (1000)      359 2024-03-12 18:47:29.400017 ceotr_git_manager-1.2.0/PKG-INFO
--rw-rw-r--   0 elliskeener-lacroix  (1000) elliskeener-lacroix  (1000)      588 2024-02-29 02:28:09.000000 ceotr_git_manager-1.2.0/README.md
-drwxrwxr-x   0 elliskeener-lacroix  (1000) elliskeener-lacroix  (1000)        0 2024-03-12 18:47:29.396017 ceotr_git_manager-1.2.0/ceotr_git_manager/
--rw-rw-r--   0 elliskeener-lacroix  (1000) elliskeener-lacroix  (1000)      197 2024-03-12 14:02:39.000000 ceotr_git_manager-1.2.0/ceotr_git_manager/GitFile.py
--rw-rw-r--   0 elliskeener-lacroix  (1000) elliskeener-lacroix  (1000)    15283 2024-03-12 18:27:07.000000 ceotr_git_manager-1.2.0/ceotr_git_manager/GitRepo.py
--rw-rw-r--   0 elliskeener-lacroix  (1000) elliskeener-lacroix  (1000)      171 2024-02-29 02:28:09.000000 ceotr_git_manager-1.2.0/ceotr_git_manager/GitUser.py
--rw-rw-r--   0 elliskeener-lacroix  (1000) elliskeener-lacroix  (1000)       87 2024-03-12 15:21:01.000000 ceotr_git_manager-1.2.0/ceotr_git_manager/__init__.py
-drwxrwxr-x   0 elliskeener-lacroix  (1000) elliskeener-lacroix  (1000)        0 2024-03-12 18:47:29.396017 ceotr_git_manager-1.2.0/ceotr_git_manager.egg-info/
--rw-r--r--   0 elliskeener-lacroix  (1000) elliskeener-lacroix  (1000)      359 2024-03-12 18:47:29.000000 ceotr_git_manager-1.2.0/ceotr_git_manager.egg-info/PKG-INFO
--rw-rw-r--   0 elliskeener-lacroix  (1000) elliskeener-lacroix  (1000)      346 2024-03-12 18:47:29.000000 ceotr_git_manager-1.2.0/ceotr_git_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 elliskeener-lacroix  (1000) elliskeener-lacroix  (1000)        1 2024-03-12 18:47:29.000000 ceotr_git_manager-1.2.0/ceotr_git_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 elliskeener-lacroix  (1000) elliskeener-lacroix  (1000)       18 2024-03-12 18:47:29.000000 ceotr_git_manager-1.2.0/ceotr_git_manager.egg-info/top_level.txt
--rw-rw-r--   0 elliskeener-lacroix  (1000) elliskeener-lacroix  (1000)        1 2024-03-06 18:21:09.000000 ceotr_git_manager-1.2.0/ceotr_git_manager.egg-info/zip-safe
--rw-rw-r--   0 elliskeener-lacroix  (1000) elliskeener-lacroix  (1000)       38 2024-03-12 18:47:29.400017 ceotr_git_manager-1.2.0/setup.cfg
--rw-rw-r--   0 elliskeener-lacroix  (1000) elliskeener-lacroix  (1000)      730 2024-03-12 18:47:08.000000 ceotr_git_manager-1.2.0/setup.py
+drwxr-xr-x   0 cotter     (501) staff       (20)        0 2024-05-06 05:42:47.724991 ceotr_git_manager-1.2.1/
+-rw-r--r--   0 cotter     (501) staff       (20)      162 2024-04-17 16:54:51.000000 ceotr_git_manager-1.2.1/LICENSE.md
+-rw-r--r--   0 cotter     (501) staff       (20)      387 2024-05-06 05:42:47.724870 ceotr_git_manager-1.2.1/PKG-INFO
+-rw-r--r--   0 cotter     (501) staff       (20)      761 2024-05-06 05:39:50.000000 ceotr_git_manager-1.2.1/README.md
+drwxr-xr-x   0 cotter     (501) staff       (20)        0 2024-05-06 05:42:47.723319 ceotr_git_manager-1.2.1/ceotr_git_manager/
+-rw-r--r--   0 cotter     (501) staff       (20)      323 2024-05-06 05:39:50.000000 ceotr_git_manager-1.2.1/ceotr_git_manager/GitFile.py
+-rw-r--r--   0 cotter     (501) staff       (20)    15201 2024-05-06 05:39:50.000000 ceotr_git_manager-1.2.1/ceotr_git_manager/GitRepo.py
+-rw-r--r--   0 cotter     (501) staff       (20)     2525 2024-05-06 05:39:50.000000 ceotr_git_manager-1.2.1/ceotr_git_manager/GitRepoGitlab.py
+-rw-r--r--   0 cotter     (501) staff       (20)     1516 2024-05-06 05:39:50.000000 ceotr_git_manager-1.2.1/ceotr_git_manager/GitRepoRemoteBase.py
+-rw-r--r--   0 cotter     (501) staff       (20)      180 2024-05-06 05:39:50.000000 ceotr_git_manager-1.2.1/ceotr_git_manager/GitUser.py
+-rw-r--r--   0 cotter     (501) staff       (20)      178 2024-05-06 05:39:50.000000 ceotr_git_manager-1.2.1/ceotr_git_manager/__init__.py
+drwxr-xr-x   0 cotter     (501) staff       (20)        0 2024-05-06 05:42:47.724485 ceotr_git_manager-1.2.1/ceotr_git_manager.egg-info/
+-rw-r--r--   0 cotter     (501) staff       (20)      387 2024-05-06 05:42:47.000000 ceotr_git_manager-1.2.1/ceotr_git_manager.egg-info/PKG-INFO
+-rw-r--r--   0 cotter     (501) staff       (20)      420 2024-05-06 05:42:47.000000 ceotr_git_manager-1.2.1/ceotr_git_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 cotter     (501) staff       (20)        1 2024-05-06 05:42:47.000000 ceotr_git_manager-1.2.1/ceotr_git_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 cotter     (501) staff       (20)       18 2024-05-06 05:42:47.000000 ceotr_git_manager-1.2.1/ceotr_git_manager.egg-info/top_level.txt
+-rw-r--r--   0 cotter     (501) staff       (20)        1 2024-04-17 16:55:52.000000 ceotr_git_manager-1.2.1/ceotr_git_manager.egg-info/zip-safe
+-rw-r--r--   0 cotter     (501) staff       (20)       38 2024-05-06 05:42:47.725033 ceotr_git_manager-1.2.1/setup.cfg
+-rw-r--r--   0 cotter     (501) staff       (20)      730 2024-05-06 05:40:32.000000 ceotr_git_manager-1.2.1/setup.py
```

### Comparing `ceotr_git_manager-1.2.0/ceotr_git_manager/GitRepo.py` & `ceotr_git_manager-1.2.1/ceotr_git_manager/GitRepo.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,96 +5,100 @@
 import datetime
 from .GitUser import GitUser
 from .GitFile import GitFile
 from typing import List
 
 logger = logging.getLogger(__name__)
 
+
 class GitException(Exception):
-    "Raised when there is a git issue"
+    """Raised when there is a git issue"""
     pass
 
+
 class GitRepo:
     def __init__(self,
                  url,
                  repo_dir,
                  user: GitUser = None,
-                 branch = "master",
+                 branch="master",
                  pull_replace_remote=True,
                  pull_replace_local=False,
                  overwrite=False):
-        '''
+        """
             Params:
                 overwrite=False: only used when using this class with the "with" keyword
-        '''
-        
+        """
+
         self.url = url
         self.repo_dir = repo_dir
         self.user: GitUser = user
         self.base_url = url
         self.branch = branch
         self.currently_committed = False
         self.pull_replace_local = pull_replace_local
         self.pull_replace_remote = pull_replace_remote
         self.overwrite = overwrite
 
         self.entered = False
 
         if pull_replace_local == pull_replace_remote:
             raise ValueError("pull_replace_local AND pull_replace_remote cannot be set to the same value")
-    
+
     @classmethod
     def from_dict(cls, config):
-        '''
+        """
             Shortcut to use a config dictionary-like object
                 Params:
                     git_user: The gituser
                     config: url: str
                             repo_dir: str
                             branch: str
                             pull_replace_remote: str
                             pull_replace_local: str
                             overwrite: bool
 
-        '''
+        """
         return cls(**config)
 
+    # private
 
-# private
-    
     def _repo_exists(self):
         return os.path.exists(self.repo_dir)
-    
+
     def _inject_credentials(self) -> str:
         return f'{self.url[:8]}{self.user.username}:{self.user.access_token}@{self.url[8:]}'
 
-
     def _run_git_cmd(self, cmd, exception_msg="") -> str:
         if type(cmd) is str:
             cmd = [cmd]
         cmd_start = ["git", "--git-dir", os.path.join(self.repo_dir, ".git"), "--work-tree", self.repo_dir]
         cmd_start.extend(cmd)
         run = subprocess.run(cmd_start, capture_output=True)
         if run.returncode != 0:
             if exception_msg == "":
                 exception_msg = " ".join(cmd_start)
-            logging.error(f"Got an error from a git command, info: \nreturn code: {run.returncode} \nstd_out: {run.stdout.decode()}")
-            raise GitException(f"Code: {run.returncode}. Something went wrong when trying to execute git command: {exception_msg}\n{run.stdout.decode()}\n{run.stderr.decode()}")
+            logging.error(
+                f"Got an error from a git command, info: \nreturn code: {run.returncode} \nstd_out: {run.stdout.decode()}")
+            raise GitException(
+                f"Code: {run.returncode}. Something went wrong when trying to execute git command: {exception_msg}\n{run.stdout.decode()}\n{run.stderr.decode()}")
         return run.stdout.decode()
 
     def _get_changed_contents(self):
         changed_files = [os.path.join(self.repo_dir, file) for file in self.get_file_changes(["M"])]
         changed_files_contents = []
         for file in changed_files:
-            with open(file, "r") as f: changed_files_contents.append(f.read())
+            with open(file, "r") as f:
+                changed_files_contents.append(f.read())
         return changed_files_contents, changed_files
-    
+
     def _write_changed_contents(self, changed_files, changed_files_contents):
         for index, file in enumerate(changed_files):
-            with open(file, "w") as f: f.write(changed_files_contents[index])
+            with open(file, "w") as f:
+                f.write(changed_files_contents[index])
 
     def _update_repo(self):
         try:
             self._run_git_cmd("pull", exception_msg="pull")
         except GitException as e:
             if "Your local changes to the following files would be overwritten by merge" in str(e):
                 print()
@@ -104,110 +108,105 @@
                 elif self.pull_replace_remote:
                     changed_files_contents, changed_files = self._get_changed_contents()
                     self._stage_files()
                     self._run_git_cmd(["stash"])
                     self._run_git_cmd(["pull"])
                     self._write_changed_contents(changed_files, changed_files_contents)
             else:
-                logger.error("Looks like you commited changes before re-pulling, why?")
+                logger.error("Looks like you committed changes before re-pulling, why?")
                 raise e
 
-
-    def _inject_credentials(self) -> str:
-        return f'{self.url[:8]}{self.user.username}:{self.user.access_token}@{self.url[8:]}'
-
     def _first_pull(self):
         repo_with_credentials = self._inject_credentials()
         cmd = f"git clone --branch {self.branch} {repo_with_credentials} {self.repo_dir}"
         subprocess.call(cmd, shell=True)
 
     def _push(self) -> bool:
         self._run_git_cmd(["push"])
         return True
-    
+
     # if files is empty it will stage all
-    def _stage_files(self, files=[]):
+    def _stage_files(self, files=None):
+        if files is None:
+            files = []
         if type(files) is str:
             files = [files]
         args = ["-A"]
         if files:
             args = files
         cmd = ["add"]
         cmd.extend(args)
         self._run_git_cmd(cmd)
 
-
     def _commit(self, message="", allow_push_fix=False):
         if not message:
             current_date_str = datetime.datetime.now().strftime("%Y-%m-%d")
             message = f"ceotr auto-commit: {current_date_str}"
         if len(message) > 50:
             logger.warning("git commit message too long, please keep it under 50 characters")
-        commit_std = self._run_git_cmd(["commit","-m",message[:50]], exception_msg="commit")
+        commit_std = self._run_git_cmd(["commit", "-m", message[:50]], exception_msg="commit")
         if "nothing to commit" in commit_std:
             logger.warning("Nothing to commit, working tree clean")
             return False
         elif "nothing added to commit but untracked files" in commit_std:
             logger.warning("untracked files found, try adding them first")
         else:
             return True
 
     def _pull(self):
         msg = self._update_repo()
         print(msg)
 
-    def _find_files(self, filename_to_search, many=True, case_senstive=True):
+    def _find_files(self, filename_to_search, many=True, case_sensitive=True):
         matched_files = []
         for root, dirs, files in os.walk(self.repo_dir):
             for filename in files:
-                if (not case_senstive and filename.lower() == filename_to_search.lower()) or \
-                    filename == filename_to_search:
-                        file_path = os.path.join(root, filename)
-                        git_file = GitFile(self.repo_dir, file_path.split(self.repo_dir)[1])
-                        if not many:
-                            return git_file
-                        matched_files.append(git_file)
+                if (not case_sensitive and filename.lower() == filename_to_search.lower()) or \
+                        filename == filename_to_search:
+                    file_path = os.path.join(root, filename)
+                    git_file = GitFile(self.repo_dir, file_path.split(self.repo_dir)[1])
+                    if not many:
+                        return git_file
+                    matched_files.append(git_file)
 
     def _add_file(self, file_path, replace, git_relative_filename="", git_relative_dirname=""):
         if (git_relative_filename == "" and git_relative_dirname == "") or \
-            (git_relative_filename != "" and git_relative_dirname != ""):
+                (git_relative_filename != "" and git_relative_dirname != ""):
             raise ValueError("Cannot set a relative filename and dirname!")
         if git_relative_dirname:
             git_relative_path = os.path.join(git_relative_dirname, file_path.split("/")[-1])
         else:
             git_relative_path = git_relative_filename
-        
+
         full_path = os.path.join(self.repo_dir, git_relative_path)
         if os.path.exists(full_path) and not replace:
-            raise FileExistsError("File exsists, and replace is set to false")
+            raise FileExistsError("File exists, and replace is set to false")
         try:
             shutil.copyfile(file_path, full_path)
         except FileNotFoundError:
             os.makedirs(os.path.dirname(full_path))
             shutil.copyfile(file_path, full_path)
         return GitFile(self.repo_dir, git_relative_path)
-    
 
     def __enter__(self):
         self.entered = True
         self.init(self.overwrite)
         return self
 
     def __exit__(self, *args):
         self.save_and_upload()
 
+    # public
 
-# public
-        
     def init(self, overwrite: bool) -> None:
-        '''
+        """
             Create or update the repo.
                 Params:
                     overwrite: overwrite the current repo with a fresh clone.
-        '''
+        """
         if overwrite and self._repo_exists():
             try:
                 print("Removing")
                 shutil.rmtree(self.repo_dir)
             except:
                 print("WARN: Could not delete repo when trying to init")
         if not self._repo_exists():
@@ -215,35 +214,36 @@
 
         else:
             current_branch = self._run_git_cmd(["branch", "--show-current"])
             if current_branch != self.branch:
                 self.change_branch(self.branch)
             self._update_repo()
             return
-        
+
         self._first_pull()
-        self._run_git_cmd(["config","--local","user.name",self.user.username])
-        self._run_git_cmd(["config","--local","user.email",self.user.email])
+        self._run_git_cmd(["config", "--local", "user.name", self.user.username])
+        self._run_git_cmd(["config", "--local", "user.email", self.user.email])
 
     def change_branch(self, branch: str) -> None:
-        '''
+        """
             Change the branch.
                 Params:
                     branch: the name of the branch to checkout to, needs to exist.
-        '''
+        """
 
         try:
             self._run_git_cmd(["checkout", branch], exception_msg="changing branch")
         except Exception as e:
             if "did not match any file(s)" in str(e):
                 raise GitException(f"Error: Cannot checkout to '{branch}'. Branch does not exist")
         self._update_repo()
 
-    def get_file_changes(self, filter=[], clean_output=True) -> List[str]: #DOESN'T WORK IF THE DIR HAS SPACES NEED FIX
-        '''
+    def get_file_changes(self, filter=[], clean_output=True) -> List[
+        str]:  # DOESN'T WORK IF THE DIR HAS SPACES NEED FIX
+        """
             Get untracked file changes on the repo:
                 Params:
                     clean_output: True - only return the file names. False - Return the character code with the file name
                     filter[]: A list of characters representing the files state
                 Returns:
                     A list of filenames for untracked changes
 
@@ -274,94 +274,92 @@
                 -------------------------------------------------
                 ?           ?    untracked
                 !           !    ignored
                 -------------------------------------------------
 
             Please use in a list, ex:   ["A", "D"]
                                         ["A"]
-        '''
+        """
         status = self._run_git_cmd(["status", "--porcelain", "--untracked-files=all"])
-        files: list = status.split("\n")[:-1] #emptyline at the end, last index is blank
+        files: list = status.split("\n")[:-1]  # empty line at the end, last index is blank
         if files:
             if filter:
                 files = [file for file in files if True in [True for substr in filter if substr in file]]
             if clean_output:
                 files = [file.split(" ")[-1] for file in files]
-        
+
         return files
-    
 
     def save_and_upload(self, files: list = [], commit_message="") -> None:
-        '''
+        """
             Stage, commit, and push changed files to the remote git repo.
                 Params:
-                    files: optional, a list of filenames to stage, if there are any filenames in this list, 
+                    files: optional, a list of filenames to stage, if there are any filenames in this list,
                             it will only stage those files to be commited and pushed.
                     commit_message: optional, the commit message.
-        '''
+        """
         self._update_repo()
         if self.get_file_changes():
             self._stage_files(files=files)
             self._commit(commit_message)
             self._push()
         else:
             logger.info("No changed files")
 
     def get_file(self, git_relative_path: str) -> GitFile:
         return GitFile(self.repo_dir, git_relative_path)
-    
-    def find_file(self, filename, case_senstive=True) -> GitFile:
-        '''
+
+    def find_file(self, filename, case_sensitive=True) -> GitFile:
+        """
             Find a file in the repo with a specific filename
                 Params:
                     filename: The filename to look for
-                    case_senstive = True: Case sensitive search
-        '''
-        return self._find_files(filename, many=False, case_senstive=case_senstive)
-    
-    def find_all_files(self, filename, case_senstive=True) -> List[GitFile]:
-        '''
+                    case_sensitive = True: Case sensitive search
+        """
+        return self._find_files(filename, many=False, case_sensitive=case_sensitive)
+
+    def find_all_files(self, filename, case_sensitive=True) -> List[GitFile]:
+        """
             Find all files in the repo with a specific filename
                 Params:
                     filename: The filename to look for
-                    case_senstive = True: Case sensitive search
-        '''
-        return self._find_files(filename, many=True, case_senstive=case_senstive)
+                    case_sensitive = True: Case sensitive search
+        """
+        return self._find_files(filename, many=True, case_sensitive=case_sensitive)
 
     def add_file(self, file_path: str, git_relative_filename="", git_relative_dirname="", replace=True):
-        '''
+        """
             Add a file to the git repo. \n
             **NOTE** this will be slow if adding multiple files and not using this class with the "with" keyword or use 'add_many_files()'
                 Params:
                     file_path: The full filename and path to add to the git repo
                     git_relative_filename: the relative filename related to the git repo
                     git_relative_dirname: the dir to add the file in, this will keep the original filename
                     replace=True: If a file with the same name exists, replace it or not
                 Returns:
                     GitFile of the added file
-        '''
+        """
         git_file = self._add_file(file_path,
-                                    replace,
-                                    git_relative_dirname=git_relative_dirname,
-                                    git_relative_filename=git_relative_filename)
+                                  replace,
+                                  git_relative_dirname=git_relative_dirname,
+                                  git_relative_filename=git_relative_filename)
         if not self.entered:
             self.save_and_upload(commit_message=f"added file: {git_file.file_relative_path}")
         return git_file
-    
 
     def add_many_files(self, file_paths: List[str], git_relative_dirname="", replace=True):
-        '''
+        """
             Add multiple files to the git repo.
                 Params:
                     file_path: The full filename and path to add to the git repo
                     git_relative_dirname: the dir to add the files into, this will keep the original filename
                     replace=True: If a file with the same name exists, replace it or not
                 Returns:
                     GitFile of the added file
-        '''
+        """
         git_files = []
         for file in file_paths:
             git_file = self._add_file(file, replace, git_relative_dirname=git_relative_dirname)
             git_files.append(git_file)
         if not self.entered:
             self.save_and_upload(commit_message=f"added files to: {git_relative_dirname}")
         return git_files
```

### Comparing `ceotr_git_manager-1.2.0/setup.py` & `ceotr_git_manager-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 path_to_my_project = os.path.dirname(__file__)  # Do any sort of fancy resolving of the path here if you need to
 
 
 install_requires = []
 packages = find_packages(exclude=['tests'])
 
 setup(name='ceotr_git_manager',
-      version='1.2.0',
+      version='1.2.1',
       description="Common python library for CEOTR data team to manage git repositories programically",
       author="CEOTR",
       author_email="support@ceotr.ca",
       url="https://gitlab.oceantrack.org/ceotr-public/ceotr_app_common/ceotr_git_manager",
       packages=packages,
       include_package_data=True,
       license="GNU General Public License v3 (GPLv3)",
```

