# Intro to Graph Convolutional Networks(GCN)
This is a test statement.
There's not particularly any "physical" meaning to the convolution operation. The main use of convolution in engineering is in describing the output of a linear, time-invariant (LTI) system. The input-output behavior of an LTI system can be characterized via its impulse response, and the output of an LTI system for any input signal x(t)x(t) can be expressed as the convolution of the input signal with the system's impulse response.

Namely, if the signal x(t)x(t) is applied to an LTI system with impulse response h(t)h(t), then the output signal is:

y(t)=x(t)∗h(t)=∫∞−∞x(τ)h(t−τ)dτ
y(t)=x(t)∗h(t)=∫−∞∞x(τ)h(t−τ)dτ
Like I said, there's not much of a physical interpretation, but you can think of a convolution qualitatively as "smearing" the energy present in x(t)x(t) out in time in some way, dependent upon the shape of the impulse response h(t)h(t). At an engineering level (rigorous mathematicians wouldn't approve), you can get some insight by looking more closely at the structure of the integrand itself. You can think of the output y(t)y(t) as the sum of an infinite number of copies of the impulse response, each shifted by a slightly different time delay (ττ) and scaled according to the value of the input signal at the value of tt that corresponds to the delay: x(τ)x(τ).

This sort of interpretation is similar to taking discrete-time convolution (discussed in Atul Ingle's answer) to a limit of an infinitesimally-short sample period, which again isn't fully mathematically sound, but makes for a decently intuitive way to visualize the action for a continuous-time system.