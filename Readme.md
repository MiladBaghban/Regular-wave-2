Example: A ship 500 feet long is moving on a regular sequence of waves at an angle of 
         40 degrees to the line of the crest of the wave. The ship's chest hits 
         successive waves every 15 seconds, and it takes 10 seconds for the tip of the 
         wave to reach from the ship's chest to the ship's heel. Find the speed of the ship. <br />
<br />
Solution: 

<image align="right" alt="Milad" width = "300" src="http://up44.ir/previews/54d2659c867de6cd83f16ff70593ea7e.jpg">
         
<pre>import math     # library of python for calculate the calculation of below <br />
µ = 50          # degree <br />
L = 500         # ship lenght <br />
t = 10          # time of passing wave from bow to stern <br />
π = 3.14        # pi number <br />
T_e = 15        # collision course <br />
g = 32.2        # gavity
H = (L * math.cos(µ)) / t    # H = (V_w - (V * math.cos(µ))) = (L * math.cos(µ))
L_w = T_e * H                # wave length
V_w = math.sqrt((g * L_w) / (2 * π))      # wave velocity
V = V_w / math.cos(µ)                     # ship velocity
print(f"(V_w - (V * math.cos(µ))) = {H:0.4f}")
print(f"L_w = {L_w:0.4f}")
print(f"V_w = {V_w:.4f}")
print(f"V = {V:0.4f}")
