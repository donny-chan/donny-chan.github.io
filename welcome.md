## Welcome to xxx

You can use the [editor on GitHub](https://github.com/Blazing-Bonfire/blazing-bonfire.github.io/edit/master/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### 现在没啥内容

可能放点Leetcode题解吧

#### 欧拉筛法
```C++
int n, cnt = 0;
int* primes = new int[n+1];  // 所有素数，升序
bool* vis = new vis[n+1];    // 记录非素数
memset(vis, false, sizeof(bool) * (n+1));
memset(primes, 0, sizeof(int) * (n+1));
for (int i = 2; i <= n; ++i) {
    if (!vis[i]) primes[cnt++] = i;
    for (int j = 0; j < cnt && i * primes[j] <= n; ++j) {
        vis[i * primes[j]] = true;    // 倍数记为非素数
        if (i % prime[j] == 0) break; // 关键，与Eratosthenes不同
    }
}
```

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/Blazing-Bonfire/blazing-bonfire.github.io/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
