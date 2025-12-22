# Git Platform Blob URL Conversion Test

Testing automatic conversion of blob URLs to raw URLs for various Git hosting platforms.

> [!TIP]
> **MarkView Advantage**: This extension automatically converts blob URLs to raw URLs for all major Git platforms (GitHub, GitLab, Bitbucket, Gitea, etc.), providing better image support than the platforms themselves. GitHub blob URLs only work natively when hosted on GitHub, and GitLab doesn't support blob URLs at all - but MarkView makes them work everywhere!

---

## 1. GitHub

> [!NOTE]
> Link to the original markdown file on GitHub: [test-git-platform-blob-urls.md](https://github.com/markview-app/sample-markdown/blob/main/samples/test-git-platform-blob-urls.md)

### Test 1: GitHub blob URL

> [!IMPORTANT]
> At the time this sample was created, GitHub supported this image link format, but only worked if this markdown file was hosted on GitHub.

<img src="https://github.com/markview-app/sample-markdown/blob/main/assets/image-1.jpg" alt="GitHub blob" height="500">

### Test 2: GitHub raw URL

<img src="https://raw.githubusercontent.com/markview-app/sample-markdown/refs/heads/main/assets/image-1.jpg" alt="GitHub raw" height="500">

### Test 3: GitHub relative URL

<img src="../assets/image-1.jpg" alt="GitHub relative" height="500">

---

## 2. GitLab

> [!NOTE]
> Link to the original markdown file on GitLab: [test-git-platform-blob-urls.md](https://gitlab.com/dangthanhtung/markview-sample-markdown/-/blob/main/samples/test-git-platform-blob-urls.md)

### Test 1: GitLab blob URL

> [!WARNING]
> At the time this sample was created, GitLab did not support this image link format.

<img src="https://gitlab.com/dangthanhtung/markview-sample-markdown/-/blob/main/assets/image-1.jpg" alt="GitLab blob" height="500">

### Test 2: GitLab raw URL

<img src="https://gitlab.com/dangthanhtung/markview-sample-markdown/-/raw/main/assets/image-1.jpg" alt="GitLab raw" height="500">

### Test 3: GitLab relative URL

<img src="../assets/image-1.jpg" alt="GitLab relative" height="500">
