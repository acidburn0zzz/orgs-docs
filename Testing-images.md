<img src="menu-choose.png" style="border: 1px solid gray;">

 NOTE: If you have changed Node.js versions and are still getting	 NOTE: If you have changed Node.js versions and are still getting
-and error on a supported version of Node.js, you may need to rebuild npm:	+an error on a supported version of Node.js, you may need to rebuild npm:
 	 
 ```	 ```
 $ npm rebuild	 $ npm rebuild
    
11  content/getting-started/semantic-versioning.md
@@ -15,7 +15,12 @@ If a project is going to be shared with others, it should start at `1.0.0`, (tho
 	 
 After this, changes should be handled as follows:	 After this, changes should be handled as follows:
 	 
-![SemVerTable](/images/sem_ver_table.png)	+| CODE STATUS  | STAGE | RULE | EXAMPLE # |
+| :----------- | :---- | :--- | :-------- |
+| First Release | New Product | Start with 1.0.0 | 1.0.0 |
+| Bug fixes, other minor changes | Patch Release | Increment the third digit | 1.0.1 |
+| New features that don't break existing features | Minor Release | Increment the middle digit | 1.1.0 |
+| Changes that break backward compatibility | Major Release | Increment the first digit | 2.0.0 |
 	 
 ## Semver for Consumers	 ## Semver for Consumers
 	 
@@ -29,6 +34,6 @@ If you were starting with a package 1.0.4, this is how you would specify the ran
 	 
 ## Learn More	 ## Learn More
 	 
-For more about using semantic versioning with package.json files, see [Chapter 5](https://docs.npmjs.com/getting-started/using-a-package.json#specifying-packages). 	+For more about using semantic versioning with package.json files, see [Chapter 5](https://docs.npmjs.com/getting-started/using-a-package.json#specifying-packages).
 	 
-For another way to label releases, learn about [npm dist tags](https://docs.npmjs.com/cli/dist-tag), and [how they relate to semantic versioning](https://docs.npmjs.com/getting-started/using-tags).	+For another way to label releases, learn about [npm dist tags](https://docs.npmjs.com/cli/dist-tag), and [how they relate to semantic versioning](https://docs.npmjs.com/getting-started/using-tags).
   
BIN  public/images/sem_ver_table.png
Deleted file not rendered
   
17  public/styles/index.styl
@@ -28,6 +28,23 @@ a
 header	 header
   background npmred	   background npmred
 	 
+table
+  border-collapse collapse
+  border-spacing 0
+  font-size 12px
+  width 100%
+  thead
+    background-color navy
+    color white
+  th
+    white-space nowrap
+  th,td
+    border 1px solid #ccc
+    padding 5px 10px
+  tr
+    &:nth-child(2n)
+      background-color #f8f8f8
+
 #www-link	 #www-link
   color white	   color white
   text-decoration none	   text-decoration none

	 
-![SemVerTable](/images/sem_ver_table.png)	+| CODE STATUS  | STAGE | RULE | EXAMPLE # |
+| :----------- | :---- | :--- | :-------- |
+| First Release | New Product | Start with 1.0.0 | 1.0.0 |
+| Bug fixes, other minor changes | Patch Release | Increment the third digit | 1.0.1 |
+| New features that don't break existing features | Minor Release | Increment the middle digit | 1.1.0 |
+| Changes that break backward compatibility | Major Release | Increment the first digit | 2.0.0 |
 	 
 ## Semver for Consumers	 ## Semver for Consumers
 	 
@@ -29,6 +34,6 @@ If you were starting with a package 1.0.4, this is how you would specify the ran
 	 
 ## Learn More	 ## Learn More
 	 
-For more about using semantic versioning with package.json files, see [Chapter 5](https://docs.npmjs.com/getting-started/using-a-package.json#specifying-packages). 	+For more about using semantic versioning with package.json files, see [Chapter 5](https://docs.npmjs.com/getting-started/using-a-package.json#specifying-packages).
 	 
-For another way to label releases, learn about [npm dist tags](https://docs.npmjs.com/cli/dist-tag), and [how they relate to semantic versioning](https://docs.npmjs.com/getting-started/using-tags).	+For another way to label releases, learn about [npm dist tags](https://docs.npmjs.com/cli/dist-tag), and [how they relate to semantic versioning](https://docs.npmjs.com/getting-started/using-tags).
   
BIN  public/images/sem_ver_table.png
Deleted file not rendered
   
17  public/styles/index.styl
@@ -28,6 +28,23 @@ a
 header	 header
   background npmred	   background npmred
 	 
+table
+  border-collapse collapse
+  border-spacing 0
+  font-size 12px
+  width 100%
+  thead
+    background-color navy
+    color white
+  th
+    white-space nowrap
+  th,td
+    border 1px solid #ccc
+    padding 5px 10px
+  tr
+    &:nth-child(2n)
+      background-color #f8f8f8
+
 #www-link	 #www-link
   color white	   color white
   text-decoration none	   text-decoration none
https://github.com/npm/docs/pull/930/files
