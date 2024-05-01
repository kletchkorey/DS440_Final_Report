# Can LLMs Reason? Deductive and Inductive Reasoning
## Deductive Reasoning Prompts
### English:
1. Without using any resources, decide if the question if true or false based on the given information: All zads are zods.
All zods are zids.
Are all zads zids?
2. Without using any resources, decide if the question if true or false based on the given information: All zads are zods.
All zods are zids.
Are all zids zads?
3. Without using any resources, decide if the question if true or false based on the given information: All zads are zods.
All zods are zids.
All zids are zads.
Are all zads zids?
4. Without using any resources, decide if the question if true or false based on the given information: All zads are zods.
All zods are zids.
All zids are zeds.
All zeds are zuds.
All zuds are zyds.
Are all zads zyds?
5. Without using any resources, decide if the question if true or false based on the given information: All zads are not zods.
All zods are not zids.
Are all zads zids?
6. Without using any resources, decide if the question if true or false based on the given information: No zads are not zods.
No zods are not zids.
Are all zads zids?
7. Without using any resources, decide if the question if true or false based on the given information: No zads are not zods.
No zods are not zids.
No zids are not zads.
Are all zads zids?
8. Without using any resources, decide if the question if true or false based on the given information: No zads are not zods.
No zods are not zids.
No zids are not zeds.
No zeds are not zuds.
No zuds are not zyds.
Are all zads zyds?
9. Without using any resources, decide if the question if true or false based on the given information: Some zads are zods.
All zods are zids.
Are all zads zids?
10. Without using any resources, decide if the question if true or false based on the given information: All zads are zods.
All zods are zids.
Some zids are zeds.
All zeds are zuds.
Are all zads zids?
### Logic language
1. Without using any resources, decide if the question if true or false based on the given information: ∀X, zad(X) -> zod(X)
∀Y, zod(Y) -> zid(Y)
∀Z, zad(Z) -> zid(Z)
2. Without using any resources, decide if the question if true or false based on the given information: ∀X, zad(X) -> zod(X)
∀Y, zod(Y) -> zid(Y)
∀Z, zid(Z) -> zad(Z)
3. Without using any resources, decide if the question if true or false based on the given information: ∀X, zad(X) -> zod(X)
∀Y, zod(Y) -> zid(Y)
∀T, zid(T) -> zad(T)
∀Z, zad(Z) -> zid(Z)
4. Without using any resources, decide if the question if true or false based on the given information: ∀X, zad(X) -> zod(X)
∀Y, zod(Y) -> zid(Y)
∀T, zid(T) -> zed(T)
∀Z, zed(U) -> zud(U)
∀F, zud(V) -> zyd(V)
∀G, zad(Z) -> zyd(Z)
5. Without using any resources, decide if the question if true or false based on the given information: ∀X, zad(X) -> ¬zod(X)
∀Y, zod(Y) -> ¬zid(Y)
∀Z, zad(Z) -> zid(Z)
6. Without using any resources, decide if the question if true or false based on the given information: ∀X, ¬¬zad(X) -> zod(X)
∀Y, ¬¬zod(Y) -> zid(Y)
∀Z, zad(Z) -> zid(Z)
7. Without using any resources, decide if the question if true or false based on the given information: ∀X, ¬¬zad(X) -> zod(X)
∀Y, ¬¬zod(Y) -> zid(Y)
∀T, ¬¬zid(T) -> zad(T)
∀Z, zad(Z) -> zid(Z)
8. Without using any resources, decide if the question if true or false based on the given information: ∀X, ¬¬zad(X) -> zod(X)
∀Y, ¬¬zod(Y) -> zid(Y)
∀T, ¬¬zid(T) -> zed(T)
∀T, ¬¬zed(T) -> zud(T)
∀T, ¬¬zud(T) -> zyd(T)
∀Z, zad(Z) -> zyd(Z)
9. Without using any resources, decide if the question if true or false based on the given information: ∃X, zad(X) -> zod(X)
∀Y, zod(Y) -> zid(Y)
∀Z, zad(Z) -> zid(Z)
10. Without using any resources, decide if the question if true or false based on the given information: ∀X, zad(X) -> zod(X)
∀Y, zod(Y) -> zid(Y)
∃T, zid(T) -> zed(T)
∀U, zed(U) -> zud(U)
∀Z, zad(Z) -> zid(Z)
### Transitive Property
1. Without using any resources, decide if the statement is true of false based on the given information, where (a) is transitive: ∀X, Y, Z:
a(X, Y) ^ a(Y, Z) -> a(X, Z)
2. Without using any resources, decide if the statement is true of false based on the given information, where (a) is transitive: ∀X, Y, Z:
a(X, Y) ^ a(Y, Z) -> a(Z, X)
3. Without using any resources, decide if the statement is true of false based on the given information, where (a) is transitive: ∀X, Y, T, Z:
a(X, Y) ^ a(Y, T) ^ a(T, Z) -> a(X, Z)
4. Without using any resources, decide if the statement is true of false based on the given information, where (a) is transitive: ∀X, Y, T, U, V, Z:
a(X, Y) ^ a(Y, T) ^ a(T, U) ^ a(U, V) ^ a(V, Z) -> a(X, Z)
5. Without using any resources, decide if the statement is true of false based on the given information, where (a) is transitive: ∀X, Y, Z:
¬a(X, Y) ^ ¬a(Y, Z) -> a(Z, X)
6. Without using any resources, decide if the statement is true of false based on the given information, where (a) is transitive: ∀X, Y, Z:
¬¬a(X, Y) ^ ¬¬a(Y, Z) -> a(X, Z)
7. Without using any resources, decide if the statement is true of false based on the given information, where (a) is transitive: ∀X, Y, Z:
¬¬a(X, Y) ^ ¬¬a(Y, Z) ^ ¬¬a(Z, X)  -> a(X, Z)
8. Without using any resources, decide if the statement is true of false based on the given information, where (a) is transitive: ∀X, Y, T, U, V, Z:
¬¬a(X, Y) ^ ¬¬a(Y, T) ^ ¬¬a(T, U) ^ ¬¬a(U, V) ^ ¬¬a(V, Z) -> a(X, Z)
## Inductive Reasoning
1. Without using any resources besides the given information: If zad was busy at 8 am on Tuesday for three weeks in a row, what can you assume about the zad at 8 am on the next Tuesday.
2. Without using any resources besides the given information: If zad was busy at 8 am on Tuesday for three weeks in a row, what can you assume about zad at 11 am on the next Tuesday.
3. Without using any resources besides the given information: If zad was busy at 8 am on Tuesday for three weeks in a row, what can you assume about zad at 8 am on the next Saturday.
4. Without using any resources besides the given information: There are zids in my pool every summer.  Will there be zids in my pool next summer?
5. Without using any resources besides the given information: There are zids in my pool every summer.  Will there be zids in my pool next winter?
6. Without using any resources besides the given information: There are zids in my pool every summer.  Will there be zods in my pool next summer?
7. Without using any resources besides the given information: If zads usually become zids, what can you assume about the next zad?
8. Without using any resources besides the given information: If zads usually become zids, what can you assume about the next zid?
9. Without using any resources besides the given information: If zads usually become zids, what can you assume about the next zod?
10. Without using any resources besides the given information: Zad is a blue zid.
All blue zids I have seen can fly.
What can you assume about zad?
11. Without using any resources besides the given information: Zad is a blue zid.
All red zids I have seen can fly.
What can you assume about zad?
12. Without using any resources besides the given information: Zad is a blue zid.
All blue zids I have seen can fly.
What can you assume about zod?
13. Without using any resources besides the given information: All zads in the area are blue.
All zads I have seen are blue.
What can you assume about zads?
14. Without using any resources besides the given information: All zads in the area are red.
All zads I have seen are blue.
What can you assume about zads?
15. Without using any resources besides the given information:All zads in the area are blue.
All zads I have seen are red.
What can you assume about red?
16. Without using any resources besides the given information: Zads exist.
I have never seen a zad but have heard about them.
What can I assume about zads?
17. Without using any resources besides the given information: Zads exist.
I have seen a zad but have no knowledge about them.
What can I assume about zads?
18. Without using any resources besides the given information: Zads exist.
I have never seen a zad nor do I have any knowledge about them.
What can I assume about zads?
19. Without using any resources besides the given information: Zads do not exist.
I have seen a zad.
What can I assume about zads?
20. Without using any resources besides the given information: Zads do not exist.
I have heard of a zad before, but never seen one.
What can I assume about zads?
21. Without using any resources besides the given information: Zads do not exist.
I have never seen a zad, but I have heard they exist.
What can I assume about zads?
## Statistical Reasoning
    
