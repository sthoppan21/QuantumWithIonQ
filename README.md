# QuantumWithIonQ

Simple QiSkit program to run a sample Circuit


from qiskit import QuantumCircuit

-- Create a basic Bell State
circuit = QuantumCircuit(2, 2) # 2 qubits, 2 bits
circuit.h(0)
circuit.cx(0, 1)

-- Measure qubits 0 and 1 into bits 0 and 1 respectively
circuit.measure([0, 1], [0, 1])

-- NOTE: circuit.measure_all() or circuit.measure_active() would do the same here

-- Display circuit, same as print(circuit.draw(output="text"))
print(circuit)


