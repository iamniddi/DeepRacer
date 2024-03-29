# Deep Racer on a Real Track

<br/><br/>

In 2022, Dong-A University and Hanoi National University jointly hosted the "Deep Racer" competition. Since this competition is not a virtual race, So our team needed a code and model that drive well on the real track.

We also needed a model to run reliably on any track because the track that we would actually compete on was private until the day of the competition.

In this situation, I would like to share some tips and experiences that our team has realized.


<br/><br/><br/>




### 1. Remember, it's not a virtual race
In a virtual race, many people calculate the shortest path of a track and make it run on that waypoint. Our team also approached it that way at first.<br/>

<p align="center"><img src="https://github.com/iamniddi/DeepRacer/assets/110338470/fb199964-296c-4279-b42e-52851118f36b" width="60%" height="60%"></p>

In a virtual environment, it worked well and set a fast record. But it was different on the actual track. The vehicle moves to the designated waypoint even if the starting point is slightly different. In other words, we can't cope with flexible situations
<br/>
There's a way to run the shortest route flexibly, but at least our team didn't find that way. So we had to abandon this strategy. 
<br/><br/><br/>


### 2. Keep the code simple
We decided to reduce the code briefly. Both virtual competitions on Amazon and competitions on real-world tracks use sophisticated but complex algorithms. It's sometimes useful, but we basically didn't know which track to run on.

<br/><br/><br/>

### 3. You have to pick a good track to learn
It's the most important strategy. The deep racer recognizes the road through the camera and selects the learned speed and direction to move.  
When you first train a model, if you train a track with various curves, even in an anomalous situation, the camera will recognize the road that has already been learned.

<p align="center"><img src="https://github.com/iamniddi/DeepRacer/assets/110338470/1be071d2-727c-470c-9bf7-c28a3c9f8cd2" width="30%" height="30%"></p>
<br/>
We found that track is "Bowie Track".There are various directions in various directions and stable than it.



Models learned from Bowie Track also run reliably on other tracks. We also confirmed that it runs steadily when it is driven on a real track.

<p align="center"><img src="https://github.com/iamniddi/DeepRacer/assets/110338470/790c1670-8ee7-42db-aa90-0e78b77f3ccc" width="60%" height="60%"></p>
<br/><br/><br/>

### 4. Calibration

Finally, you need to adjust the "calibration" of the deep racer machine, but it's really sensory-dependent. Prepare the vehicle and track, change the value little by little, and find the right value


<br/><br/><br/>
### Our model

After two hours of learning with the code I put up, It showed a stable, upward graph. And as a result, our team won.
<p align="center"><img src="https://github.com/iamniddi/DeepRacer/assets/110338470/6b5a4531-6863-4630-ab32-9af23948f43a" width="60%" height="60%"></p>
<br/><br/>

<p align="center">

<img src="https://github.com/iamniddi/DeepRacer/assets/110338470/f0fd1eb1-ef9f-44c8-9f54-0f452895796c">

</p>

<p align="center">

<img src="https://github.com/iamniddi/DeepRacer/assets/110338470/5c13bb3c-1987-48bf-9bd2-71de1df51245)">

</p>

<br/><br/><br/>



### review of the competition

In 2022, we went to Hanoi, Vietnam. Received hospitality from Hanoi National University. I was lucky to win. Hanoi was a wonderful city


2023 now. Students from Hanoi National University came to Korea this time. I participated in the competition again this time and put a lot of effort into it, and paid for the aws server cost with my own money.

However, I was suddenly informed by the university that I could not participate in the competition. I was not apologised for my efforts and expenses, and everything went to nothing. I had the worst experience. I don't want this to happen again

Fortunately, my team without me won the championship, and I felt rewarded

<br/><br/><br/>

### 2022 team members
<br/>

[Jung JaeYoung](https://github.com/recordpang)

[Jung Heechul](https://github.com/IronPower9K)
