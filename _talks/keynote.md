---
name: Converging towards generality
number: keynote
speakers:
  - Anders Schou Simonsen
categories:
  - Plenary
---

Simulating physical phenomena in real-world applications poses significant challenges. However, leveraging the right computational tools can enable efficient and accurate modelling. In this keynote presentation, I will present my approach to solving complex, coupled systems, with a focus on the numerical methods employed. Specifically, I will present a MATLAB-based solver I've developed, designed to allow users to input equations in a flexible, EES-like manner (where expressions can be defined interchangeably on the left- or right-hand side). The solver utilizes symbolic mathematics to automatically linearize these equations and assemble them into large sparse matrices, enabling rapid convergence even for intricate coupled systems. Additionally, I will explore the application of linear programming techniques to optimize such systems effectively.
Beyond model development, ensuring usability through an intuitive interface is equally crucial. I will showcase the PureSim platform, an online tool I’ve initiated at Alfa Laval, where users can interact with these models directly in their web browser. This approach leverages modern web technologies, and I will demonstrate the strategies and methodologies employed to create a seamless user experience.
