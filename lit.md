# Simulation of life in a 2D world: A Literature Review 

## Introduction

With the rising of AI, more and more gaming developers are paying attention to adding AI feature into their games. The development of AI-based video games has gained significant attention in recent years due to the potential of AI to enhance gameplay and provide a more immersive experience for players. AI-based games can provide players with more challenging opponents and dynamic gameplay that adapts to their actions, which can lead to a more satisfying gaming experience. The development of an AI-based 2D game can contribute to the advancement of the field by demonstrating the potential of AI to enhance gameplay and create more sophisticated gaming experience. In the computer game we developed within the scope of the study, AI abilities were used in order for the game characters to survive as long as possible, to use the most advanced equipment, to successfully complete various stages of the game, and to develop more advanced game tactics. (Ayas, 2023) Now, with the power of AI, we can create a kind of NPC (non-player-character) that has ai brain. Therefore, we decided to create a 2D world to create an area where simulates lives in a 2D world. In this literature review, we will dive deeply into the necessary methods and strategies of developing this project.

The development of AI-based video games has gained significant attention in recent years due to the potential of AI to enhance gameplay, provide a more immersive experience for players, and create more sophisticated gaming experience. AI-based games can provide players with more challenging opponents and dynamic gameplay that adapts to their actions, which can lead to a more satisfying gaming experience.

Also, AI-based games contribute to the simutation of biological life, such as micelium, ants, and other creatures.

## Different Approaches to AI in Games

There are several different approaches to implementing AI in games, each with its own strengths and weaknesses. One common approach is to use rule-based systems, which involve creating a set of rules that govern the behavior of AI characters in the game. These rules can be simple or complex, depending on the desired behavior of the characters. Another approach is to use machine learning techniques, such as neural networks, to train AI characters to behave in a certain way. This approach can be more flexible than rule-based systems, as it allows the AI characters to learn from their environment and adapt their behavior accordingly. A third approach is to use a combination of rule-based systems and machine learning techniques to create more sophisticated AI characters that can exhibit complex behaviors.

### Rule-Based Systems

Rule-based systems are a common approach to implementing AI in games and involve creating a set of rules that govern the behavior of AI characters in the game. These rules can be simple or complex, depending on the desired behavior of the characters. For example, if a game is 2D celluar automata, the rules can be simple, such as "if a cell has fewer than two neighbors, it dies; if it has more than three neighbors, it dies; if it has exactly three neighbors, it is born." In these cases, the rules are simple and deterministic, and the behavior of the AI characters may adapt to the environment (Adami & Brown, 1994). Rule-based systems can be effective for creating AI characters that exhibit specific behaviors, such as following a path, avoiding obstacles, or attacking enemies. However, they can be limited in their ability to adapt to changing environments or learn from experience.

### Machine Learning Techniques

Machine learning techniques, such as neural networks, can be used to train AI characters to behave in a certain way. This approach can be more flexible than rule-based systems, as it allows the AI characters to learn from their environment and adapt their behavior accordingly. For example, a neural network can be trained to recognize patterns in the environment and respond to them in a certain way. This approach can be more complex than rule-based systems, as it requires training data and a learning algorithm to train the neural network. However, we can use machine learning techniques to create more sophisticated AI characters that can exhibit complex behaviors. For example, we can create a colony simulation in which AI characters that will have better brains will survive, and the others will die out. Also, they can make babies and evolve. (Ian Millington, 2019)

### Hybrid Approaches

A third approach is to use a combination of rule-based systems and machine learning techniques to create more sophisticated AI characters that can exhibit complex behaviors. This approach can combine the strengths of both rule-based systems and machine learning techniques, allowing the AI characters to exhibit specific behaviors while also learning from their environment and adapting their behavior accordingly. For example, we can use a rule-based system to create a set of rules that govern the behavior of AI characters in the game (in general), and then use machine learning techniques to add unpredictability to the AI characters' behavior.

## AI-Based Game Development

There are three main elements here: allocating execution time among the artificial intelligence that needs it, having algorithms that can work a little at once on several frames, and prioritizing important roles when resources are scarce. The level of detail algorithms in artificial intelligence are no different from those in graphics: from the player's perspective, they prioritize computer time to allocate to the most important or error prone roles. By combining frequency and priority scheduling, problems caused by scheduling can be reduced; Building robust and reusable world interfaces using two different technologies: event passing and polling, most AI specific design tools are related to basic technologies: finite state machines or behavior trees, motion, and pathfinding. The toolchain is naturally better at allowing designers to modify data rather than code, so the use of classic techniques is being strengthened. The toolchain approach to developing games places a responsibility on the content creation team to provide necessary AI knowledge. This process can be assisted by offline processing, which automatically generates a knowledge database from the original level information. Most level editing tools and all 3D modeling tools allow users to add invisible helper objects at a certain point. The support of arbitrary boundary regions in level design or modeling tools is complex. Therefore, this method is often simplified to placing arbitrarily aligned bounding boxes.

### Game Engine

To develop a video game, we need to use a poper game engine to start our projects. Game engines combine all the physical mechanisms, graphics components, libraries, and scripts (pieces of code) into one game; they are the most basic programs that control the input and output in the game. The most basic function of game engines is to provide input from the user. These input devices vary depending on the platform for which the game is written. General-purpose game engines adapt all of these input libraries so that the game maker does not have to write optimized code for each input device. One of the most important tasks of game engines is to create game graphics and draw them. (Ayas, 2023)

Also, we can make an engine in Python using Pygame library. Pygame is a set of Python modules designed for writing video games. Pygame adds functionality on top of the excellent SDL library. This allows you to create fully featured games and multimedia programs in Python. Pygame is highly portable and runs on nearly every platform and operating system. Pygame itself has been downloaded millions of times, and has had millions of visits to its website. (Sadli, 2022)

Our approach is to write a game engine in C++ using SFML library. For brain development, we can use Python and its libraries, such as TensorFlow, PyTorch, or Keras, and then integrate the brain into the game engine using exposed API.

### Graphics

In order to develop a video game, we nned to decide the graphic style and graphic elements. While developing the game, we are supposed to set up and design all the graphic properties to make the game visible. For character oriented games, the designer should design all the possible graphic elements to interact with the character. For instance: the environment, the NPCs, the mobs, the map, and the status.


### Leveling

In order to control the game, the collected data is used to create a level, which affects the type and difficulty of the level. The statistical characteristics such as how often the player jumped, died, how much he caught Renga cannot be 
directly controlled by the game because of they depend on the player’s skill and playing style. In the tests, the game levels for a particular player have been dynamically generated as:

1. A first level is generated with random parameters.

2. Game features are recorded.

3. Using recorded game features

, a new adapted level is generated based on player experience. (Schneider, 2009)


## Colonies Simulation

The most typical example of a colony simulation is the ant colony simulation.

There may be environment, in which the creatures live. The environment may have some resources, such as sugar, water, earth elevations, walls and predators. The creatures' behavior may be implemented as a set of basic defensive mechanisms (Schneider & Rosa, 2009).

## Conclusion

In this review, we have discussed the different approaches to implementing AI in games, including rule-based systems, machine learning techniques, and hybrid approaches. We have also discussed the development of AI-based games and the use of game engines to create video games. We have also discussed the development of a colony simulation in which AI characters can exhibit complex behaviors.

We decided to create a 2D world to simulate live of creatures in a 2D world. We will use a combination of rule-based systems and machine learning techniques to create more sophisticated AI characters that can exhibit complex behaviors. We want to create a colony simulation in which AI characters that will have better brains will survive, and the others will die out; basically, we want to use machine learning techniques to implement the evolution of the creatures in our game.

## References

- Ayas, M. (2023). AI-Based 2D Game Development. Journal of Game Development, 1(1), 1-10.
Cetin, M., & Sarıca, Y. (2020). Artificial Intelligence Based Game Levelling. Balkan Journal of Electrical and Computer Engineering, 8(2), 147-153. https://doi.org/10.17694/bajece.642973

- Schneider, M. O., & Rosa, J. L. G. (2009). Application and development of biologically plausible neural networks in a multiagent artificial life system. Neural Computing and Applications, 18(1), 65–75. https://doi.org/10.1007/s00521-007-0156-0

- Adami, Christoph & Brown, C. Titus. (1994). Evolutionary Learning in the 2D Artificial Life System "Avida". Artifical Life IV.

- Sadli, Adi. (2022). Using The Python Library to Create Simple Game Animations. International Journal of Management Science and Information Technology. 2. 21-31. 10.35870/ijmsit.v2i2.699.

- Millington, Ian. (2019). AI for Games. 10.1201/9781351053303. 


