This page contains answers to frequently asked questions, which are not addressed elsewhere in our [documentation](http://leagueofrobotrunners.org/resources). If you have additional questions, or require further clarifications, please drop by our [Discord channel](https://discord.gg/CEYT4g4raR). You can also email the organisers at **league-of-robot-runnners [at] googlegroups [dot] com** (although Discord is usually faster).

## Frequent Questions ![r11](external_page_resource/robots/r11_s.png)

**Q: Can I modify the start kit code?**

> No, except for the bits that we explicitly tell you to modify in the start-kit instructions.

**Q: Can one team join the competition with multiple github accounts?**

> No

**Q: Can I be part of more than one team?**

> No

**Q: My team used up all of our training award credits, can we have more?**

> The total number of training awards is limited and for this reason we normally allocate only one award per team. If you believe your situation is exceptional in some way, please email us (although the answer is probably no). 

**Q: Will my implementation been reviewed by organisers?**

>Yes, the organisers will review participants' implementation at the end of the competition.

**Q: How to work with multiple collaborators?** 
>To work as a team, only one team member need to create a team on the website. The team leader can then fill in the team members' details and github usernames in the team page. The team leader can also give the team members access to the team's submission repository using the "Repo Manage" tab.

**Q: My score on the leaderboard has decreased! Why?**

> If another participant has improved a best-known solution then existing submissions will be re-scored relative to this new baseline. More details about our scoring function are available on the [evaluation](https://leagueofrobotrunners.org/evaluation) page.

**Q: A timestep is equal to one second, but my planner always takes less than 1 second to compute actions. Can I benefit from the time saved, so I can be evaluated for more timesteps?**

> Finishing before the time limit per timestep is fine. But you cannot "bank" the time saved. This is because we always evaluate your planner up to a fixed planning horizon, measured in timesteps. 

**Q: What does the Evaluation Base Docker Image in my submission panel mean?**

> The Evaluation Base Docker Image is the docker image that will be used to build the evaluation environment for your submission. This is the docker image that will be used to run your planner. We give following options for the Evaluation Base Docker Image:
> **PyTorch Docker Images**:
> - [pytorch/pytorch:2.5.1-cuda11.8-cudnn9-devel](https://hub.docker.com/layers/pytorch/pytorch/2.5.1-cuda11.8-cudnn9-devel/images/sha256-676c7b7423d7e726b814b98cfd5b702e1b32016b2e0ef0270f6202a6c660c419), Ubuntu 22.04 with PyTorch 2.5.1, CUDA 11.8, and cuDNN 9.
> - [pytorch/pytorch:2.5.1-cuda12.1-cudnn9-devel](https://hub.docker.com/layers/pytorch/pytorch/2.5.1-cuda12.1-cudnn9-devel/images/sha256-e8e63dd7baca894ba11fe1ba48a52a550793c8974f89b533d697784dd20a4dc0), Ubuntu 22.04 with PyTorch 2.5.1, CUDA 12.1, and cuDNN 9.
> - [pytorch/pytorch:2.5.1-cuda12.4-cudnn9-devel](https://hub.docker.com/layers/pytorch/pytorch/2.5.1-cuda12.4-cudnn9-devel/images/sha256-14611869895df612b7b07227d5925f30ec3cd6673bad58ce3d84ed107950e014), Ubuntu 22.04 with PyTorch 2.5.1, CUDA 12.4, and cuDNN 9.
> **NVIDIA CUDA Docker Images**:
> - [nvidia/cuda:12.6.3-cudnn-devel-ubuntu20.04](https://hub.docker.com/layers/nvidia/cuda/12.6.3-cudnn-devel-ubuntu20.04/images/sha256-41b64c7236c0ff59f11298584676b4af95c0ddf9924f18c6072b160fddd6c34f), Ubuntu 20.04 with CUDA 12.6.3 and cuDNN 9.
> - [nvidia/cuda:12.6.3-cudnn-devel-ubuntu22.04](https://hub.docker.com/layers/nvidia/cuda/12.6.3-cudnn-devel-ubuntu22.04/images/sha256-cb239b67719dfa32ec6b525b54c1b78559bebd51a47249dd702f6c5429372154), Ubuntu 22.04 with CUDA 12.6.3 and cuDNN 9.
> - [nvidia/cuda:12.6.3-cudnn-devel-ubuntu24.04](https://hub.docker.com/layers/nvidia/cuda/12.6.3-cudnn-devel-ubuntu24.04/images/sha256-0f8250615943f311785f9ce6379a49520a4b53c124d22b42ba859edf93af3991), Ubuntu 24.04 with CUDA 12.6.3 and cuDNN 9.
> **TensorFlow Docker Images**:
> - [tensorflow/tensorflow:2.18.0-gpu](https://hub.docker.com/layers/tensorflow/tensorflow/2.18.0-gpu/images/sha256-1f16fbd9be8bb84891de12533e332bbd500511caeb5cf4db501dbe39d422f9c7), Ubuntu 22.04 with TensorFlow 2.18.0 and CUDA 12.3.
> - [tensorflow/tensorflow:latest-gpu](https://hub.docker.com/layers/tensorflow/tensorflow/latest-gpu/images/sha256-1f16fbd9be8bb84891de12533e332bbd500511caeb5cf4db501dbe39d422f9c7), the latest TensorFlow GPU image.
> **Ubuntu Docker Images**:
> - [ubuntu:jammy](https://hub.docker.com/layers/library/ubuntu/jammy/images/sha256-3d1556a8a18cf5307b121e0a98e93f1ddf1f3f8e092f1fddfd941254785b95d7), Ubuntu 22.04.
