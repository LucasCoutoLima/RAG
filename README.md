# Sistema de RAG combinando busca e LLMs

Esse projeto foi feito para a disciplina de mestrado da Unicamp IA024 - Redes Neurais Profundas para Processamento de Linguagem Natural.

Neste projeto, foi construído um sistema RAG para responder perguntas do Dataset IIRC (Incomplete Information Reading Comprehension) utilizando informações de documentos, buscando os documentos mais relevantes para cada pergunta e gerando as respostas com base nos documentos.

O trabalho foi dividido da seguinte maneira:

- Etapa 1: Segmentação do texto
- Etapa 2: Computação das embeddings e indexação - A ideia é usar busca densa, usando um modelo de embeddings para criar representações vetoriais para os segmentos obtidos na etapa 1. FAISS foi utilizado para criar e gerenciar os índices dos documentos.
- Etapa 3: Geração das respostas (prompt), LLM utilizado foi o Llama 3.1 70b com a API da groq.com
- Etapa 4: Avaliação, F1-bag-of-words e Exact Match.
