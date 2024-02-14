# RoboClinician
## Inspiration
The Turing Test, initially proposed by Alan Turing in 1950 as the "Imitation Game," evaluates a machine's ability to exhibit intelligent behavior indistinguishable from that of a human. In 1991, Hugh Loebner initiated the Loebner Prize competition, offering a $100,000 prize for the first computer program to pass an unrestricted Turing Test, with annual competitions for the best program in a restricted version. And then there was Tinymuds, Tinymuds played a significant role in the development of a Turing System that participated in the first three Loebner Prize competitions, focusing on its design, performance, and the enhancement through a four-year development process fueled by online community engagement. Tiny muds achieved the below three points: multiplayer conversation, textual “scenery” simulating physical spaces user extensibility

Decades later we have the Large Language Models, which primarily work on the idea of generating next token or next word prediction, to be simply put and the chatGPT which now have a 175B parameter multi-modal running at their backend. But there are specialised LLMs which can be used by medical professionals, including physicians and students, as they often juggle vast amounts of information, making it challenging to consistently draw connections. ChatGPT is not explicitly tailored for medical inquiries, particularly those pertaining to diagnosis or symptoms. Moreover, the critical requirement for contextual understanding necessitates that patient data remain confidential, in line with doctor-patient privacy standards, and should not be transmitted to the OpenAI API. Therefore, our goal is to establish a platform that enables medical practitioners, students, and researchers to swiftly obtain accurate and relevant answers to their queries.

## What it does
It answers questions aimed at medical queries through specialised LLMs and it does not uses chatGPT.

## How we built it
Our system was meticulously crafted with a backend powered entirely by open-source Large Language Models, ensuring comprehensive and responsive question-answering capabilities. The front end is supported by a robust combination of HTML, CSS, and Django to provide a seamless user experience. We used the 7B version of Meditron: https://huggingface.co/epfl-llm/meditron-7b

## Challenges we ran into
Accommodating a model of this magnitude presents its own set of challenges. With nearly 7 billion parameters, these models are relatively smaller than ChatGPT, yet they demand a substantial array of GPUs to sustain their operations effectively.

## Accomplishments that we're proud of
A fully opensourced framework which can be used by medical practioners, clinicians and students alike. We are proud that we are not just another chatGPT wrapper.

## What we learned
Handling LLMs at scale!! both at the backend and at the UI level!

## What's next for RoboClinician
Compression aka Quantization of the models and redesigning the UI to fit to smaller devices like watch/raspberryPI/AR devices.

## Built With
1. cuda
2. HTML
3. CSS
4. flask
5. huggingface
4. python
