##论文简介
* Generating Supplemental Content Information Using Virtual Profiles (Page 295)
    * linkedin公司出品，从一些用户的基本信息中得到更多的格外信息。
    * ABSTRACT
    We describe a hybrid recommendation system at LinkedIn that seeks to optimally extract relevant information pertaining to items to be recommended. By extending the notion of an item proﬁle, we propose the concept of a “virtual proﬁle” that augments the content of the item with rich set of features inherited from members who have already shown explicit interest in it. Unlike item-based collaborative ﬁltering, we focus on discovering the characteristic descriptors that underlie the item-user association. Such information is used as supplemental features in a content-based ﬁltering system. The main objective of virtual proﬁles is to provide a means to tap into rich-content information from one type of entity and propagate features extracted from which to other aﬃliated entities that may suﬀer from relative data scarcity. We empirically evaluate the proposed method on a real-world community recommendation problem at LinkedIn. The result shows that the virtual proﬁles outperform a collaborative ﬁltering based approach (user who likes this also likes that). In particular, the improvement is more signiﬁcant for new users with only limited connections, demonstrating the capability of the method to address the cold-start problem in pure collaborative ﬁltering systems.    
    * Categories and Subject Descriptors H.2.8 [Database Management]: Data Mining 
    * Keywords hybrid recommender systems; feature generation and extraction; model-based recommendation; virtural proﬁles
   


* Nonlinear Latent Factorization by Embedding Multiple User Interests (Page 65)
    * google出品，讲通过用户的行为的矩阵来抽取隐语义
    * ABSTRACT:
    Classical matrix factorization approaches to collaborative ﬁltering learn a latent vector for each user and each item, and recommendations are scored via the similarity between two such vectors, which are of the same dimension. In this work,we are motivated by the intuition that a user is a much more complicated entity than any single item, and cannot be well described by the same representation. Hence, the variety of a user’s interests could be better captured by a more complex representation. We propose to model the user with a richer set of functions, speciﬁcally via a set of latent vectors,where each vector captures one of the user’s latent interests or tastes. The overall recommendation model is then nonlinear where the matching score between a user and a given item is the maximum matching score over each of the user’s latent interests with respect to the item’s latent representation. We describe a simple, general and eﬃcient algorithm for learning such a model, and apply it to large scale, realworld datasets from YouTube and Google Music, where our approach outperforms existing techniques.
    * Keywords:
	collaborative ﬁltering, learning to rank, matrix factorization,nonlinear models   

##有关图的论文
* Trading-off Among Accuracy, Similarity, Diversity, and Long-tail: A Graph-based Recommendation Approach
    * 百度出品，讲到理论和现实的折中，这一篇打算重点阅读一下
    * Trading-off Among Accuracy, Similarity, Diversity, and Long-tail: A Graph-based Recommendation Approach
    * ABSTRACT：
    Improving recommendation accuracy is the mostly focused target of recommendation systems, while it has been increasingly recognized that accuracy is not enough as the only quality criterion. More concepts have been proposed recently to augment the evaluation dimensions, such as similarity, diversity, long-tail, etc. Simultaneously considering multiple criteria leads to a multi-task recommendation. In this paper, a graph-based recommendation approach is proposed to effectively and ﬂexibly trade-off among them. Our approach is considered based a 1st order Markovian graph with transition probabilities between user-item pairs. A “cost ﬂow” concept is proposed over the graph, so that items with lower costs are stronger recommended to a user. The cost ﬂows are formulated in a recursive dynamic form, whose stability is proved to be guaranteed by appropriately lower-bounding the transition costs. Furthermore, a mixture of transition costs is designed by combining three ingredients related to long-tail, focusing degree and similarity. To evaluate the ingredients, we propose an orthogonal-sparseorthogonal nonnegative matrix tri-factorization model and an effcient multiplicative algorithm. Empirical experiments on real-world data show promising results of our approach, which could be regarded as a general framework for other affects if transition costs are designed in various ways. 
    * Categories and Subject Descriptors H.3.3 [Information Storage and Retrieval]: Information Search and Retrieval—Information Filtering General Terms Algorithm, Proof, Experimentation, Performance
    * Keywords:
    Collaborative ﬁltering, graph-based cost ﬂow, ﬁxed point stability, contraction mapping, orthogonal-sparse-orthogonal nonnegative matrix tri-factorization
    

* DrunkardMob: Billions of Random Walks on Just a PC (Page 257)
    * graphchi是我一直看好的项目，也许有一天集群会被小型的，随身携带的机器学习一体机所取代。关注graphChi    
    * ABSTRACT：Random walks on graphs are a staple of many ranking and recommendation algorithms. Simulating random walks on a graph which fits in memory is trivial, but massive graphs pose a problem: the latency of following walks across network in a cluster or loading nodes from disk on-demand renders basic random walk simulation unbearably inefficient. In this work we propose DrunkardMob, a new algorithm for simulating hundreds of millions, or even billions, of random walks on massive graphs, on just a single PC or laptop. Instead of simulating one walk a time it processes millions of them in parallel, in a batch. Based on DrunkardMob and GraphChi [19], we further propose a framework for easily expressing scalable algorithms based on graph walks.
    * Keywords：recommender systems, random walks, graph computation


* Cross Social Networks Interests Predictions Based on Graph Features (Page 319)
    * 当前各种SNS，人们在不同的sns上留下了不同的印记。如何将一个人在不同的sns上的信息整合到一起，给他进行跨品类的推荐。 
    * ABSTRACT:The tremendous popularity of Online Social Networks (OSN) has led to situations, where users have their profiles spread across multiple networks. These partial profiles re ect different user characteristics, depending mainly on the nature of the network, e.g., Facebook's social vs. LinkedIn's professional focus. Combining data gathered by multiple networks may benefit individual users, and the community as a whole, as this could facilitate the provision of more accurate services and recommendations. This paper reports on an exploratory study of the process of making such recommendations using a unique multi-network dataset containing user interests across multiple domains, e.g., music, books, and movies. We represent the data using a graph model and generate recommendations using a set of features extracted from and populated by the model. We assess the contribution of various network- and domain-related features to the accuracy of the recommendations and motivate future work into automated feature selection.
    * Categories and Subject Descriptors:H.3.3 [Information Storage and Retrieval]: Information Filtering
    * Keywords:Social Networks; Graph Model; Interests Prediction


* Recommending Scientific Articles Using Bi-Relational Graph-based Iterative RWR (Page 399)
    * 利用二分图给科研工作者提供科学论文的推荐
    * ABSTRACT:The overabundance of scientiﬁc article information has created much inconvenience to researchers seeking interesting articles online. In this paper, we provide a Bi-Relational graph to represent the heterogenous information of scientiﬁc article recommendation system, which includes three parts: the article content similarity, researcher interest correlation, and researcher-article readership. Meanwhile, an iterative random walk with restarts learning method is proposed on the Bi-Relational graph to recommend a researcher rating for each article by making use of the known information. The proposed method has ability to perform both old and new article recommendation. A series of experiments on CiteULike dataset have shown that our method is more eﬀective than other testing methods in the paper.
    * Categories and Subject Descriptors:H.3 [Information Storage and Retrieval]: Information Search and Retrieval—Information ﬁltering; I.2 [Artiﬁcial Intelligence]: Learning
    * Keywords:Recommending scientiﬁc article, Bi-Relational Graph, Iterative RWR, New article recommendation, Old article recommendation


* Leveraging the Citation Graph to Recommend Keywords (Page 359)
    * 利用论文的引用关系图来推测一篇论文它的keywords应该是什么，和这个论文实际的keywords进行比较
    * ABSTRACT:Users of scienti¯c papers databases, such as CiteSeerX, Google Scholar, and Microsoft Academic, often search for papers using a set of keywords. Unfortunately, many authors avoid listing su±cient keywords for their papers. As such, these applications may need to automatically associate good descriptive keywords with papers. This is a well-studied problem given the complete text of the paper, but in many cases,due to copyright privileges, research papers databases do not have the complete text, only metadata, such as the title and abstract. On the other hand, research papers databases typically maintain the citation network of each paper. In this paper we study the problem of predicting which keywords are appropriate for a scienti¯c paper, using only the citation network. We compare our method with predicting keywords using the title and abstract, concluding that the citation network provides much better predictions.
    * Categories and Subject Descriptors:H.4 [Information Systems Applications]: Miscellaneous
    * Keywords:Keywords Recommendation, Citation Graph, Academic Papers


* A Heterogeneous Graph-Based Recommendation Simulator (Page 471)
    * 还没有理解，看起来像是一篇工程性的，将一个模拟器的框架
    * ABSTRACT:Users of scienti¯c papers databases, such as CiteSeerX, Google Scholar, and Microsoft Academic, often search for papers using a set of keywords. Unfortunately, many authors avoid listing su±cient keywords for their papers. As such, these applications may need to automatically associate good descriptive keywords with papers. This is a well-studied problem given the complete text of the paper, but in many cases,due to copyright privileges, research papers databases do not have the complete text, only metadata, such as the title and abstract. On the other hand, research papers databases typically maintain the citation network of each paper. In this paper we study the problem of predicting which keywords are appropriate for a scienti¯c paper, using only the citation network. We compare our method with predicting keywords using the title and abstract, concluding that the citation network provides much better predictions.
    * Categories and Subject Descriptors:H.4 [Information Systems Applications]: Miscellaneous
    * Keywords:Keywords Recommendation, Citation Graph, Academic Papers



* 邮件:weiweijiuzaizhe@gmail.com
* QQ: weiweijiuzaizhe@gmail.com
* weibo: [@吴炜_数据挖掘机器学习]http://weibo.com/u/2770304367)

<!--注释掉
##捐助开发者
在兴趣的驱动下,写一个`免费`的东西，有欣喜，也还有汗水，希望你喜欢我的作品，同时也能支持一下。
当然，有钱捧个钱场（右上角的爱心标志，支持支付宝和PayPal捐助），没钱捧个人场，谢谢各位。

##感激
感谢以下的项目,排名不分先后

* [mou](http://mouapp.com/) 
* [ace](http://ace.ajax.org/)
* [jquery](http://jquery.com)

##关于作者

```javascript
  var ihubo = {
    nickName  : "草依山",
    site : "http://jser.me"
  }
```
-->