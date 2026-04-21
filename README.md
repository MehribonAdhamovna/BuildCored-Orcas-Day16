# BuildCored-Orcas-Day16
EchoKiller — BUILDCORED ORCAS Day 16

What it does. This code listens to a sound that has an echo, uses math to "guess" what that echo looks like, and then subtracts it from the signal in real time. It’s basically a digital eraser that identifies repeating patterns and rubs them out so the audio stays clear.

Hardware concept. This represents Acoustic Echo Cancellation (AEC), the same technology used in your smartphone's speakerphone or an Amazon Echo. In hardware a dedicated chip (DSP) does this math instantly so you don't hear your own voice bouncing back when you're on a call.

Screen Recording. https://drive.google.com/file/d/16kn0HW_QHeUS87Mkg4T9fC3s-pqUlnyu/view?usp=sharing

What I would do differently. To improve this for a real world scenario, I would use a Normalized LMS (NLMS) or a frequency domain filter to handle louder noises without the audio breaking. I would also increase the filter order even further to account for "reverb" which is just many tiny echoes bouncing off walls instead of just one big one.

Run it. python day16_starter.py
