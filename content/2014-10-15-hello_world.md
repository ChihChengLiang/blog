title: Hello world
date: 2014-10-15
comments: true
slug: hello_world

![successful kid]({filename}/images/hello_world_pic.jpg)

Finally the blog is up! 

Thanks to Gilbert's great article  [http://weichengliou.github.io/blog/blog/2014/08/07/buildblog/](http://weichengliou.github.io/blog/blog/2014/08/07/buildblog/) . Also thanks to the following original toturial too.

- [http://jakevdp.github.io/blog/2013/05/07/migrating-from-octopress-to-pelican/](http://jakevdp.github.io/blog/2013/05/07/migrating-from-octopress-to-pelican/)
- [http://ocefpaf.github.io/python4oceanographers/blog/2013/12/23/blog/](http://ocefpaf.github.io/python4oceanographers/blog/2013/12/23/blog/)

Now I have a blog that can embed ipython notebook cells.

{% notebook nbtest.ipynb cells[:] %}


Here is some additional info on setup of pelican, which might save you some time.

- When things get ugly, don't hesitate to `make clean` or `rm output/ -r`. Some bugs ,`'ascii' codec can't decode byte 0xe6 in position 80: ordinal not in range(128)` for example, that you might not know where to fix, lives in the `output/` directory. 
- If you want to build your own blog by hacking an existing blog repository, `python4oceanographers` for examle, do reinitialize the git repository first! Else, You will find the first `git push` takes forever after the deletion of the existing posts. 
- Make sure your `cells` in `{％ notebook nbtest.ipynb cells[1:] %}` refers to the correct cells in the ipynb file. (Sorry for that fullwidth percentage sign, one does not simply escape the variable delimiters in pelican)

