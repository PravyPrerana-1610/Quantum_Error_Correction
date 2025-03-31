Classical Computing:-   
    Classical computers have bits such as 8 bits,32 bits or 64 bits.

Quantum Computing:-
   
$|\Psi\rangle = \sum_{i=0}^{2^n-1} c_i |i\rangle, \quad c_i \in \mathbb{C}, \quad \sum_{i=0}^{2^n-1} |c_i|^2 = 1$.  
Here, $c_i$ represent the amplitudes of $|i \rangle$ 's and modulo square of these amplitudes give us the prboability of $\Psi$ being in a given particular state. Also, the probabilities ,ust sum upto 1.

# Quantum Gates
1. Bit flip gate   
$X$ flips the qubit from $\lvert 0 \rangle \rightarrow \lvert 1 \rangle$ and $\lvert 1 \rangle \rightarrow \lvert 0 \rangle$.       
If there is a superposition of more than one qubits as below then it permutes amplitudes.           
$\alpha \lvert 000 \rangle + \beta \lvert 111 \rangle  \xrightarrow{X_0}  \alpha \lvert 001 \rangle + \beta \lvert 110 \rangle$        
$\alpha \lvert 000 \rangle + \beta \lvert 111 \rangle  \xrightarrow{X_2}  \alpha \lvert 100 \rangle + \beta \lvert 011 \rangle$        
$\alpha \lvert 000 \rangle + \beta \lvert 111 \rangle  \xrightarrow{X_2}  \alpha \lvert 100 \rangle + \beta \lvert 011 \rangle$
2. Phase flip gate 
This leaves $\lvert 0 \rangle$ unchanged but it changes the sign of $\lvert 1 \rangle$.         
$\alpha \lvert 000 \rangle + \beta \lvert 111 \rangle  \xrightarrow{Z_2}  \alpha \lvert 000 \rangle - \beta \lvert 111 \rangle $        
$\alpha \lvert 000 \rangle + \beta \lvert 111 \rangle  \xrightarrow{Z_1}  \alpha \lvert 000 \rangle - \beta \lvert 111 \rangle $        
$\alpha \lvert 000 \rangle + \beta \lvert 111 \rangle  \xrightarrow{Z_0}  \alpha \lvert 000 \rangle - \beta \lvert 111 \rangle $


Quantum circuits provide away to represent these gates and states as input. It has one line for each qubit. And gates are applied to the state from left to right.

<figure>
  <img src="/Users/pravyprerana/Desktop/PHD codes/Quantum_Error_Correction/2BEB5B03-4087-4200-9BB0-1CDF961ABF50.jpeg" width="400">
  <figcaption> This circuit shows the initial state and the gates act upon them from bottom to top. </figcaption>
</figure>