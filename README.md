## Work progress

The plan for today was: 
- Assist to the seminar from Yann Olivier about information theory in Deep Learning
- Try to talk to Yann Olivier about his publication about RNNs with no backProp
- Bring the registration papers to EDITE
- Validate my list of courses for PIF

All the paper work (registration and courses) was successfully done

## The small resume of the seminar:

The talk was mainly about what learning is from mathematical point of view and the relashions between information theory and Neural Networks.

Mathematical theory to describe what learning is - by Kolmogoroff and Solomonoff in 60s. Impossible to implement in real life.

Def. a definition of object X is a computer program that prints X

K(X) = shortest length of such a program - Kolmogoroff complexity

Learning can be concidered as compression - reducing the dimensionalty of data. When learning we try to smallest possible representation of our data, without redundencies and taking in the account all regularities.

Several bounds can be pointed out when talking about Kolmogoroff complexity:
1) K(f(x)) <= K(x) + K(f) + const, where f is a re-encoding

2) Let K_1 and K_2 be the Kolmogoroff complexities wrt 2 programming languages. Then there exists C12 | for each x |K_1(x) - K_2(x)| <= C12. C12 can be considered as the size of the interpreter between K_1 and K_2.

3) K(x) <= length(x) + length("print") + 2*log(length(x))

4) K(x) <= length(zip(x)) + length(unzip)

5) If x is an element or subset of E, then K(x) <= K(E) + log(|E|)

6) For any probability distribution p, K(x) <= K(p) + log(1/p(x))

M(x, y) = K(x) + K(y) - K(xy) can be considered as a measure of distance between x and y (analogue of enthropy)

Then followed a small introduction of Neural Networks. Points, that were interesting for me: 
1) NN can theoretically represent any possible function.
2) From statistical (and complexity) point of view having amodel with more parameters than the available data size has no sense.
3) Small introduction to variational methods to overcome over-fitting. The goal is not just to find weight of NN where the solution is "good", but find weights that are "good" with their whole epsilon-environment.

Then small intro to auto-encoders and its application to natural language processing and translation was made.



