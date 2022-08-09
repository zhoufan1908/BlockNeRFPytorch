# Weekly Neural Radiance Fields [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

## Jul31 - Aug6, 2022
- [NFOMP: Neural Field for Optimal Motion Planner of Differential Drive Robots With Nonholonomic Constraints, IEEE Robotics and Automation Letters](https://ieeexplore.ieee.org/abstract/document/9851532/) | [code]
    > Optimal motion planning is one of the most critical problems in mobile robotics. On the one hand, classical sampling-based methods propose asymptotically optimal solutions to this problem. However, these planners cannot achieve smooth and short trajectories in reasonable calculation time. On the other hand, optimization-based methods are able to generate smooth and plain trajectories in a variety of scenarios, including a dense human crowd. However, modern optimization-based methods use the precomputed signed distance function for collision loss estimation, and it limits the application of these methods for general configuration spaces, including a differential drive non-circular robot with non-holonomic constraints. Moreover, optimization-based methods lack the ability to handle U-shaped or thin obstacles accurately. We propose to improve the optimization methods in two aspects. Firstly, we developed an obstacle neural field model to estimate collision loss; training this model together with trajectory optimization allows improving collision loss continuously, while achieving more feasible and smoother trajectories. Secondly, we forced the trajectory to consider non-holonomic constraints by adding Lagrange multipliers to the trajectory loss function. We applied our method for solving the optimal motion planning problem for differential drive robots with non-holonomic constraints, benchmarked our solution, and proved that the novel planner generates smooth, short, and plain trajectories perfectly suitable for a robot to follow, and outperforms the state-of-the-art approaches by 25% on normalized curvature and by 75% on the number of cusps in the MovingAI environment.

- [NeSF: Neural Semantic Fields for Generalizable Semantic Segmentation of 3D Scenes](https://research.google/pubs/pub51563/) | [code]
    > We present NeSF, a method for producing 3D semantic fields from pre-trained density fields and sparse 2D semantic supervision. Our method side-steps traditional scene representations by leveraging neural representations where 3D information is stored within neural fields. In spite of being supervised by 2D signals alone, our method is able to generate 3D-consistent semantic maps from novel camera poses and can be queried at arbitrary 3D points. Notably, NeSF is compatible with any method producing a density field, and its accuracy improves as the quality of the pre-trained density fields improve. Our empirical analysis demonstrates comparable quality to competitive 2D and 3D semantic segmentation baselines on convincing synthetic scenes while also offering features unavailable to existing methods.

- [PRIF: Primary Ray-based Implicit Function](https://research.google/pubs/pub51556/) | [code]
    > We introduce a new implicit shape representation called Primary Ray-based Implicit Function (PRIF). In contrast to most existing approaches based on the signed distance function (SDF) which handles spatial locations, our representation operates on oriented rays. Specifically, PRIF is formulated to directly produce the surface hit point of a given input ray, without the expensive sphere-tracing operations, hence enabling efficient shape extraction and differentiable rendering. We demonstrate that neural networks trained to encode PRIF achieve successes in various tasks including single shape representation, category-wise shape generation, shape completion from sparse or noisy observations, inverse rendering for camera pose estimation, and neural rendering with color.

- [Transformers as Meta-Learners for Implicit Neural Representations, ECCV2022](https://arxiv.org/abs/2208.02801) | [code](https://yinboc.github.io/trans-inr/)
    > Implicit Neural Representations (INRs) have emerged and shown their benefits over discrete representations in recent years. However, fitting an INR to the given observations usually requires optimization with gradient descent from scratch, which is inefficient and does not generalize well with sparse observations. To address this problem, most of the prior works train a hypernetwork that generates a single vector to modulate the INR weights, where the single vector becomes an information bottleneck that limits the reconstruction precision of the output INR. Recent work shows that the whole set of weights in INR can be precisely inferred without the single-vector bottleneck by gradient-based meta-learning. Motivated by a generalized formulation of gradient-based meta-learning, we propose a formulation that uses Transformers as hypernetworks for INRs, where it can directly build the whole set of INR weights with Transformers specialized as set-to-set mapping. We demonstrate the effectiveness of our method for building INRs in different tasks and domains, including 2D image regression and view synthesis for 3D objects. Our work draws connections between the Transformer hypernetworks and gradient-based meta-learning algorithms and we provide further analysis for understanding the generated INRs.

- [End-to-end learning of 3D phase-only holograms for holographic display](https://www.nature.com/articles/s41377-022-00894-6) | [code]
    > Computer-generated holography (CGH) provides volumetric control of coherent wavefront and is fundamental to applications such as volumetric 3D displays, lithography, neural photostimulation, and optical/acoustic trapping. Recently, deep learning-based methods emerged as promising computational paradigms for CGH synthesis that overcome the quality-runtime tradeoff in conventional simulation/optimization-based methods. Yet, the quality of the predicted hologram is intrinsically bounded by the dataset’s quality. Here we introduce a new hologram dataset, MIT-CGH-4K-V2, that uses a layered depth image as a data-efficient volumetric 3D input and a two-stage supervised+unsupervised training protocol for direct synthesis of high-quality 3D phase-only holograms. The proposed system also corrects vision aberration, allowing customization for end-users. We experimentally show photorealistic 3D holographic projections and discuss relevant spatial light modulator calibration procedures. Our method runs in real-time on a consumer GPU and 5 FPS on an iPhone 13 Pro, promising drastically enhanced performance for the applications above.

- [VolTeMorph: Realtime, Controllable and Generalisable Animation of Volumetric Representations](https://arxiv.org/pdf/2208.00949) | [code]
    > The recent increase in popularity of volumetric representations for scene reconstruction and novel view synthesis has put renewed focus on animating volumetric content at high visual quality and in real-time. While implicit deformation methods based on learned functions can produce impressive results, they are `black boxes' to artists and content creators, they require large amounts of training data to generalise meaningfully, and they do not produce realistic extrapolations outside the training data. In this work we solve these issues by introducing a volume deformation method which is real-time, easy to edit with off-the-shelf software and can extrapolate convincingly. To demonstrate the versatility of our method, we apply it in two scenarios: physics-based object deformation and telepresence where avatars are controlled using blendshapes. We also perform thorough experiments showing that our method compares favourably to both volumetric approaches combined with implicit deformation and methods based on mesh deformation.

- [Controllable Free Viewpoint Video Reconstruction Based on Neural Radiance Fields and Motion Graphs, IEEE Transactions on Visualization and Computer Graphics](https://ieeexplore.ieee.org/abstract/document/9845414) | [code]
    > In this paper, we propose a controllable high-quality free viewpoint video generation method based on the motion graph and neural radiance fields (NeRF). Different from existing pose-driven NeRF or time/structure conditioned NeRF works, we propose to first construct a directed motion graph of the captured sequence. Such a sequence-motion-parameterization strategy not only enables flexible pose control for free viewpoint video rendering but also avoids redundant calculation of similar poses and thus improves the overall reconstruction efficiency. Moreover, to support body shape control without losing the realistic free viewpoint rendering performance, we improve the vanilla NeRF by combining explicit surface deformation and implicit neural scene representations. Specifically, we train a local surface-guided NeRF for each valid frame on the motion graph, and the volumetric rendering was only performed in the local space around the real surface, thus enabling plausible shape control ability. As far as we know, our method is the first method that supports both realistic free viewpoint video reconstruction and motion graph-based user-guided motion traversal. The results and comparisons further demonstrate the effectiveness of the proposed method.

- [Robust Change Detection Based on Neural Descriptor Fields, IROS2022](https://ieeexplore.ieee.org/abstract/document/9845414) | [code](https://yilundu.github.io/ndf_change)
    > In this paper, we propose a controllable high-quality free viewpoint video generation method based on the motion graph and neural radiance fields (NeRF). Different from existing pose-driven NeRF or time/structure conditioned NeRF works, we propose to first construct a directed motion graph of the captured sequence. Such a sequence-motion-parameterization strategy not only enables flexible pose control for free viewpoint video rendering but also avoids redundant calculation of similar poses and thus improves the overall reconstruction efficiency. Moreover, to support body shape control without losing the realistic free viewpoint rendering performance, we improve the vanilla NeRF by combining explicit surface deformation and implicit neural scene representations. Specifically, we train a local surface-guided NeRF for each valid frame on the motion graph, and the volumetric rendering was only performed in the local space around the real surface, thus enabling plausible shape control ability. As far as we know, our method is the first method that supports both realistic free viewpoint video reconstruction and motion graph-based user-guided motion traversal. The results and comparisons further demonstrate the effectiveness of the proposed method.

## Old papers:
Refer to the [awesome-NeRF code repo](https://github.com/yenchenlin/awesome-NeRF).