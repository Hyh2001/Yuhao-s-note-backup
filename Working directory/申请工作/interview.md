# problems

1. 自我介绍
2. 各段研究经历以及其中值得提的点（有挑战的地方，有困难怎么克服的）（表现motivation）
## 3. CV，PS中的内容

4. 专业基本知识
5. Future career
6. 读完PHD之后想去干什么？

# preparation

1. 提前半个小时在线
2. 水，纸笔，餐巾纸
3. 用电脑
4. 确保网络通畅
5. 穿着得体
6. 把思维导图，论文草稿打开，zotero打开
7. 记得发thanks letter


# 自我介绍

Dear Prof. Xiong, it is really nice to meet you. I think it is the first time we meet face to face and I am really excited. My name is Yuhao Huang and you can see the precise Chinese words in my ppt. I major in electromechanical engineering  in the university of Macau and I am from Guang Zhou. My high school is GuangDong experimental high school. I think that I am a logical and patient people. I spent 14 years of my life learning calligraphy, 6 years on drawing and 4 years on tennis and basketball. They shaped me. In my mind, research is just like a topic I mentioned above and I treat them as a long-distance running. I want to be a better self each day after. My mother used to tell me a sentence that came from her PHD supervisor: if you are still a monk one day, then you should go and strike your bell without thinking more. At the first glance I think that this not such an active attitude and dose not show great enthusiasm on research. However, with my project develops, I think that the most important thing for me is to concentrated more on the process of research itself and be persisted. Be a better self is the most important for me. And this sentence mostly suits my requirement. I focus more on the journey I have gone through. This is also the aim of me if I have the chance to purse my PHD with you. I want to develop a solid tool sets on robot control and planning and legged robotics with you. Research skills and an in-depth understanding of robotics are also what I am chasing for. And also, I think that this is also the reason why we are compatible. Your words written for prospective students give me an impression that you know what exactly a student like me want. 

# 为什么选择机器人，为什么选择control and planning，为什么选择足式机器人？

As I have said in my SOP, I am interested in interdisciplinary fields which can combine both mechanical, electrical and computer engineering technologies.

As I have also said in my SOP, I believe that control and planning problems are core to the whole robotics field. If I want to build a real world robotics product that can perform real world moves, these problems can not be avoided. These problems will provide knowledge of every aspect of robotics to me. This feature is suitable for being a leader.

I need to admit that I am not so familiar with legged robot and I do not have many experiences. Based on my understanding, dynamical walking is an area that requires many complex algorithms to keep balance and perform moves. I believe that when learning, work on the most difficult  things will broaden my choices in the future.

# 为什么选择熊老师

I think that there are several reasons. First, I am really interested in your area. For me, an appropriate research area is more important than school title. Second, I believe that Prof. Xiong is the rising star in your area. I have compared the new professors that have been admitted to CMU RI especially the professor that are Asian people. For I have no abilities to judge the real value of some researches, I just compare the journals or conferences the papers have been published. The result is that Prof. Xiong you are as competitive as them. Another comparison I have made is between you and the new AP's in the same area of bipedal locomotion especially Prof. Ayonga, Professors in Umichigan, professors in Georgia tech... I think you are quite competitive as well. 

# 之前做过什么项目，细节是什么？

I have finished one project and two projects are ongoing. The project I have finished is about designing a soft sensor that can be used to detect human motions based on recyclable materials. I took part in the project quite late and the major part has been done. My work is to program Arduino to collect data for finishing a demo. The demo is to detect whether and how long a man has sat on a chair. The major part of the program is to perform analog to digital conversion, calculate time consuming and pass the data to an app called “Blynk” which is used in IOT and visualize the data on phones. There are two major difficulties. The first is about the time estimation part. Because the output of our sensor is not stable, therefore sometimes the time counting algorithm will be wrongly activated which will make the counted time biased from the real time consumed. I solved this problem by setting some delays in the program. 3 loops are ideal because we have tested that the whole program loops one time will cause 200ms. If the time delay is too long, then time shown to us will have one second delay.                                       The second is about the communication between Arduino and our mobile phone.  This problem is an unsolved one for me. I have finished the communication between Arduino and our mobile phone by using Wifi. However, I have discussed this with my collaborator and he proposed a problem that in some situations, our sensor may needed to be used under circumstance with no wifi. Therefore we decide to use Bluetooth to reimplement the function. I went through the documentation of our board which is called Arduino 33 Nano IoT and it supports BLE which is the low power version Bluetooth. However, when I was running the offered typical examples, it gives the result that it can not find a package which seems from its name is an internal package of Arduino. Therefore after reading the documentation for hardware, I figured out that the board is using Esp32 as its communication module. Therefore I changed to the typical program for standard Esp32 boards and it seems that Arduino has used its own API to replace the standard one and all the configurations have been written into its own configuration file. Therefore I went through all the pages talking about this board and can find nothing. At last we just give it up. I think that this problem somewhat reminds me to get more in-depth understanding of what we are using.  Another thing is that if I came across this problem now, I will mail the support engineers directly and ask help from them. At that time I just forgot this choice. 


After this project, I have taken part in a project aiming at designing a new fault diagnosis system using piezoelectret sensors and machine learning algorithms. I took part in the whole process. My major work is in machine learning side. I built models and trained them. I think that major gain during this project is that I figured out what types of research I am interested in working on. I am interested in working on researches that have both theory side and implementation side. Guided by intuitions and mathematical inductions and use them to build some new algorithms is the theory side that interest me a lot. There are several burdens and I want to introduce one that mostly influenced our project. At the very first beginning, we have tired to fuse the signal of our sensors and try to prove that our sensor networks can produce high precisions. However, we have tried several several machine learning algorithms and several feature extraction methods. They do not give good results. The precisions dose not provide higher accuracies. When I was testing the data, I have observed that even though the data fusion did not provide higher accuracies, they also did not provide lower one. The accuracy is just fluctuation around a single sensor. Therefore, I guess that if we train a model for each data individually, they will also provide a good result. Therefore I use the most basic algorithm: SVM to test. It seems like I am right. 
Also, I got many inspirations from the work of my professor. His best publications are two papers published on science robotics. The topic is about building a cockroach like soft piezoelectric robot. This is also the primary reason why I am interested in joining in his lab. Actually my lab journey starts from a lab aiming at pure programming projects. Their major projects are CV, 3D point cloud and reinforcement learning for robot arms. I have spent nearly three months in the lab and my project is about learning deep learning and implement some open source projects to get more familiar with ROS. 
# 从之前的项目中获得的感想？

Thanks to Prof. Zhong, I have gained a chance to join in a research program thoroughly. The biggest gain for this experience is that I have figured out what types of researches am I interested in. This several days when I was writing my paper for fault diagnosis system, I tried to meditate about the merits and flaws I have made during the research. When we were previously reading papers to consolidate our ideas, we did not give some considerations to the basic knowledge of vibrations. At that time, we thought that we did not need them because we just directly fed the data to machine learning algorithms. However, up to now I believe that if we want to do some meaningful researches, a solid base is needed. Even if we use machine learning algorithms, we still need to first perform signal processing and feature extraction to first get some ideas about our data.
