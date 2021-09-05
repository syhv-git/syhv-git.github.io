---
layout: project
type: project
image: images/pokedex.jpg
title: Pokedex
permalink: projects/pokedex
# All dates must be YYYY-MM-DD format!
date: 2020-12-10
labels:
  - Learning
  - Games
  - C++
summary: Create a Pokedex with children of the abstract Pokemon class
---

This programing project was the final homework assignment for ICS 212 at the University of Hawai\`i at Manoa. This was my favorite assignment in the course, as it had a fun concept, and was the most comprehensive assessment of C++. The final project for the course was actually a bit tamer in terms of C++ procedures, and I think this code demonstrates my coding style and abilities better than the final project. Also, we completed the final project prior to the last homework, and did not learn some data structures such as vectors. I enjoyed learning C and C++, and these languages helped me branch my personal research into new languages.

The main concept for this homework assignment was utilizing the vector structure to create a Pokedex which contains multiple children of the abstract Pokemon class. Vectors in C++ can be thought of as an array of objects, and are manipulated by vector modifiers. This program can also be further enhanced with more defined Pokémon and Pokémon stats/attack abilities, and potential for single monitor duels is possible, but it would require a bit of programming and manipulation of the Pokémon objects. The project can be accessed [here](https://github.com/syhv-git/pokedex).

There are currently only three children of the abstract Pokemon class, Arceus, Charizard, and Mewtwo, and each only contains the type and height of each Pokemon. As stated above, more data can be easily created for each Pokemon, and more Pokemon can be easily created with a header file and the corresponding cpp class file. If you choose to create more, do not forget to add the appropriate header files to the correct files. As for the battle idea, one could create a battle class, where attack and hit point modifications based on the hierarchy of types can be calculated. The Makefile is to simplify the compilation process, and if any files are added, one should make the correct modifications to the Makefile, to compile the project correctly. The command 'make pokedex' will sufficiently compile all subclass files and create the executable named pokedex.
