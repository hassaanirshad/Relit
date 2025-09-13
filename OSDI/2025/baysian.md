# Bayesian Code Diffusion for Efficient Automatic Deep Learning Program Optimization

## Abstract
We introduce Bayesian code diffusion, a new deep learning
program optimization strategy devised to accelerate the auto-
tuning process of deep learning compilers. Using the concepts
of prior and posterior distributions in the Bayesian frame-
work and reformulating them in the context of deep learn-
ing program optimization, the proposed approach efficiently
searches for optimal program code in a significantly reduced
search space through an iterative diffusion of program code.
To further enhance the efficiency of program optimization,
we propose pre-training and fine-tuning for the cost model,
which improves both the model’s predictive accuracy and
training efficiency. We implement Bayesian code diffusion
in Ansor and evaluate its performance on a wide range of
deep learning models on both CPUs and GPUs. Existing ap-
proaches struggle to reliably generate high-performing deep
learning programs, i.e. achieving low program execution la-
tency, across various configurations, including diverse deep
learning model architectures and hardware platforms (CPU
and GPU). In contrast, Bayesian code diffusion reduces the
end-to-end compilation (optimization) time required to gener-
ate the equivalent program execution latency in various con-
figurations, i.e., achieving up to 3.31×optimization speedup.
This substantial improvement demonstrates that Bayesian
code diffusion performs efficient and principled deep learning
program optimization across a wide range of deep learning
models, operators, and hardware (CPU and GPU).

## People
Ulsan National Institute of Science and Technology (UNIST)