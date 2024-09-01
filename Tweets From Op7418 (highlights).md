- Author:: [[@op7418 on Twitter]]
- Full Title:: Tweets From Op7418
- URL:: https://twitter.com/op7418
- Recommended By::
- Tags:: #Tweets #Inbox #Readwise
- ### Highlights first synced by #Readwise [[December 7th, 2023]]
    - 这一天还是来了，deepsex-34b，一个专门用来写小黄书（NFSW）的 LLM。下面是训练过程：

◆作者先收集了大约4GB的各种轻小说的总集合，并使用BERT对数据集中情节相似的小说进行了两轮相似性去重。此外，还混入了一部分不适宜内容的小说，以提高模型的不适宜内容识别能力。
◆然后使用YI-34B-base作为模型的基础，使用r=64 alpha=128的设置，并使用qlora对连续预训练进行3个时期的微调。
◆准备limarp+pippa数据集，将其清理为alpaca格式，并使用goliath-120b进行评分，该模型擅长角色扮演，筛选出高质量的问题和答案对。共有30k条数据。
◆使用2中获得的基础模型的数据，在6个时期内进行sft，r=16 alpha=32进行微调。

模型下载：https://t.co/HxPogfZzzx<img src='https://pbs.twimg.com/media/GAqkfOga0AAkUOM.jpg'/> ([View Tweet](https://twitter.com/op7418/status/1732377907795013749))
