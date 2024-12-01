# JitPack Publish
- How to publish android library (gradle 8.0 onwards)
- Please follow the steps below

## Just 4 step
### Step 1: Create file <a href="https://github.com/MCT-LIB/JitPackPublish/blob/main/jitpack.yml">jitpack.yml</a> (same level as project path)
### Step 2: Create file <a href="https://github.com/MCT-LIB/JitPackPublish/blob/main/github-jitpack-publish.gradle">github-jitpack-publish.gradle</a> (same level as library path)
### Step 3: Config your library (copy below code to your library gradle)
<pre>
apply from: './github-jitpack-publish.gradle'

GithubJitPackPublish {
    it.userName = "{github-username}"
    it.repositoryName = "{repository-name}"
    it.version = "1.0.0" (optional)
    it.release = true (optional)
}
</pre>

### Step 4: Almost done
- Push code to github
- Create new tag and release
- Go to https://jitpack.io and search your library

### Well done
- Please star this project if you find it useful.
