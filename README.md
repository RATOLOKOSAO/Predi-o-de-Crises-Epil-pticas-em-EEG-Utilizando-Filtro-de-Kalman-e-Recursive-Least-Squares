# Predição de Crises Epilépticas em EEG Utilizando Filtro de
Kalman e Recursive Least Squares
Seizure prediction using Kalman Filter and RLS algorithms. A comparative study on real-time EEG signal processing, feature extraction, and embedded systems feasibility.

Este projeto apresenta uma análise comparativa entre o Filtro de Kalman e o algoritmo Recursive Least Squares (RLS) aplicados à detecção antecipada de crises epilépticas, focando em sistemas de baixo custo computacional e tempo real.

📌 ResumoO trabalho utiliza a base de dados CHB-MIT para avaliar a transição entre os estados interictal e pré-ictal. Os resultados demonstraram que o Filtro de Kalman é superior para esta tarefa, alcançando:SPR (Taxa de Predição): 35,77%Lag Médio (Antecipação): 84,2 segundosEficiência: Margem de segurança de >1000x para execução em sistemas embarcados.

🛠️ Tecnologias e AlgoritmosLinguagem: PythonAlgoritmos: Filtro de Kalman (Estimador Recursivo Ótimo) e RLS.Processamento de Sinais: Extração de Features (Entropia, Energia, Variância e MAV).

📊 Principais ResultadosO Filtro de Kalman superou o RLS por manter o termo de inovação sensível a anomalias, enquanto o RLS, por sua rápida adaptação, tende a suprimir o sinal da crise.Destaque: Com um limiar de $\sigma = 2,0$, o sistema oferece o melhor equilíbrio clínico entre sensibilidade e taxa de falsos alarmes.

🚀 Como Executar
1- Clone o repositório.
2- Instale as dependências: pip install -r requirements.txt.
3- Execute o script principal: python src/main.py.
