---
layout: post
title: Primer post
excerpt: Aprende muchas cosas en este primer post.
date: 2017-04-25
tags: [Primer post]

comments: true
mathjax: true
---


Phasellus maximus, neque ac varius volutpat, eros leo aliquam leo, sit amet lobortis nunc libero in arcu. Cras sagittis commodo tellus eget hendrerit. Integer risus tellus, tincidunt nec rhoncus vel, ultricies eu sem. Aliquam dui eros, euismod ut nulla ac, pretium luctus dolor. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec tempus magna nec sapien venenatis efficitur. Proin diam quam, tincidunt quis rutrum vitae, tristique quis nibh.

Vivamus diam leo, tincidunt eu commodo in, ultricies sit amet diam. Curabitur felis mi, dictum ac convallis sit amet, venenatis ac neque. Vivamus non erat rutrum, porttitor felis quis, porta quam. Sed vel nulla arcu. Suspendisse in dolor ante. Morbi accumsan non massa eget placerat. Aliquam eu nisi at dui dignissim gravida at nec quam. Suspendisse pellentesque quis justo nec sagittis. Phasellus cursus congue odio, egestas suscipit purus tincidunt nec.


{% highlight python %}
def binary_dataset(X, y, colors=None, autoscale=True, **kwargs):
    """Plot a binary dataset."""
    colors = colors or ("#FF5C5C", "#5C5CFF")
    colors = np.asarray(colors)
    
    ax = plt.gca()
    ax.set_autoscale_on(autoscale)

    classes = y.flatten().astype(int)
    classes[classes == -1] = 0
    scatter = plt.scatter(X[:, 0], X[:, 1],
                          c=colors[classes],
                          zorder=10,
                          s=50, linewidth=0.25, marker= 'o')
    plt.margins(x=0., y=0.)
    return scatter
{% endhighlight %}


## Lorem

Nam quis ante ac sem *tincidunt suscipit*. Suspendisse vel mi purus. Nam vitae elit id ligula viverra vestibulum quis non ligula. Proin volutpat pulvinar velit, vel mattis purus efficitur nec. Nam vulputate nisl at ex pellentesque congue quis tincidunt nulla. Phasellus a metus vitae arcu mattis ultricies ac at leo. Sed augue sem, scelerisque id felis eget, sagittis tempus metus.

Fusce at **elementum eros**, in bibendum felis. Fusce ac libero fringilla, pulvinar felis eu, pharetra mauris. Cras eget facilisis lectus. Donec ullamcorper placerat suscipit. Nunc ac sapien quis ligula eleifend fringilla. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Cras sed urna mi. Maecenas lacinia, ex ac cursus hendrerit, diam dui tristique sapien, eget fringilla nisi mi id turpis. Aenean dapibus eros at est suscipit, non interdum metus bibendum.


{% highlight python %}
print("np.sign( 3) =", np.sign(3))
print("np.sign( 0) =", np.sign(0))
print("np.sign(-2) =", np.sign(-2))
{% endhighlight %}

 Cras id ornare risus, non accumsan orci.

{% highlight none %}
np.sign( 3) = 1
np.sign( 0) = 0
np.sign(-2) = -1
{% endhighlight %}

Curabitur volutpat convallis mauris, non gravida sapien posuere ut. Duis fringilla, enim ut molestie venenatis, tellus erat pretium dui, vitae interdum nisi purus ut lorem. Pellentesque bibendum fermentum turpis, volutpat lacinia nisi suscipit quis. In ac auctor nibh. Nulla ultricies tempus ipsum non auctor. Aliquam eget sem fermentum, consectetur diam id, pharetra orci. Cras id ornare risus, non accumsan orci. Curabitur nec bibendum lectus. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae;

Mauris varius lacus in sapien feugiat mollis. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Nunc risus erat, feugiat a sagittis eu, finibus eu ex. Curabitur ut consequat nisi, at facilisis sapien. Curabitur tempus enim in sodales tempor. Integer egestas est a neque malesuada, non finibus orci commodo. Curabitur ut diam ac lacus scelerisque auctor. Sed sollicitudin felis eu tempor malesuada. Donec ut erat vel elit pulvinar aliquam. Praesent tincidunt tortor turpis, eget laoreet tortor mattis nec.

$$
{\displaystyle \operatorname {sgn}(x)=\left \{ {
\begin{array}{rcl}
 1 & {\mbox{si}} & x>0\\
 0 & {\mbox{si}} & x=0\\
-1 & {\mbox{si}} & x<0
\end{array}}
\right.}
$$

Lorem ipsum dolor sit amet, `consectetur adipiscing` elit. Pellentesque mi ipsum, feugiat vel leo non, laoreet lobortis lectus. Quisque vitae lobortis neque, ut hendrerit orci. Sed nec elit et nulla aliquet auctor ut sit amet mauris. Aliquam ullamcorper nibh eros, eu euismod felis placerat non. Praesent bibendum leo purus, ac placerat libero lobortis nec. Cras nibh enim, mollis eget vulputate non, tincidunt ac nisl. Donec ut tellus vel lectus vestibulum bibendum. Curabitur tincidunt quis neque quis consequat. Integer sagittis ac tortor nec dignissim. Fusce sed nisi non massa maximus lobortis. Morbi lacinia diam ac felis auctor congue. Integer ultrices ac est in volutpat. Pellentesque lacinia orci nec augue sodales, ut accumsan metus porttitor. Cras nec risus vel arcu luctus venenatis id in nulla. Aenean ut bibendum arcu. Pellentesque at fermentum velit, non placerat sapien.
