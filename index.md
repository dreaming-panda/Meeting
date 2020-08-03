## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/dreaming-panda/Meeting/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

Diary_AIR_SCC tsinghua 2020/8/3


2020/8/3会议记录

# 1 参数选择问题:
    memory_intensive 和 compute_intensive的分类可能不是很有意义, 而配对更加关心的是对带宽的使用和程序可扩展能力,因此在调度中需要选择更有效的参数.并且还需要设计一个多级调度机制,并且设置相应的阀值.kiv,osv记录的内容随之改变.
# 2 通信方式问题:
    对于有些程序,如果连续调用众多kernel用现有的系统调用机制会引发很大的overhead, 所以需要更换通信方式.
# 3  Scheduler设计问题:
    如果遇到一个程序,有很长的cpu段,并且后面跟随一个kernel,那么在运行cpu部分时,站在kiv的角度应该如何看待这一部分程序? 如果直接将其看成后面kernel所具有的kiv的某一位,可能会引发这个机制性能的下降.
# 4  系统设计问题:
     如有必要,可以在GPU上再设计一个调度器,使得可以在GPU上实现更加细粒度的划分.

# 任务:
# 1 修改OS调度器的设计(支持多级调度),并参考相关论文,设置阈值
# 2 重新选取调度任务,完善论文motivation部分的配图.


**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/dreaming-panda/Meeting/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
