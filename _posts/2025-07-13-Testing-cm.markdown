---
layout: post
title: "Content Management Test"
date: 2025-07-13
categories: learning
---

# Learning CM with Jekyll
Inserting text after a headline, creating **special** text and so forth. 

{% highlight python %}
def main():
    
    start = time.time()
    
    ########### --- defining parsing args (automated parsing)--- ##########

    parser = argparse.ArgumentParser(description="TexGen Export to NASMAT conversion")
    parser.add_argument("inp_file_mesh", type=str, help="Path to the inp file")
    parser.add_argument("--plot_trigger",type=bool,default=False,help="Determines if plots of the ruc surfaces are output")
    ########### --- defining parsing args (manual input)--- #########
    parser.add_argument("--threadCount", type=int, default=8, help="informs the multiprocessing thread count")

    # Parse the arguments

    args = parser.parse_args()
    threadCount = args.threadCount
    mesh_filePath = args.inp_file_mesh
    start_keyword = "*Node"
    start_keyword_2 = "*Element"
    start_keyword_3 = "*ElSet, ElSet=Matrix"
    stop_pattern = r"\*\w+|^\*+$"
    plot_trigger = args.plot_trigger
{% endhighlight %}

Lets try posting this page with a simple push to remote.