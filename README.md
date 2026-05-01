# Entrega aula - Pensamento-computacional e abstrações
   
O Tema: Organização de uma Viagem Internacional
1. Níveis de Abstração
O planejamento de uma viagem de grande porte pode ser compreendido através de três camadas de complexidade crescente:

Nível Operacional (Execução de Tarefas):
Este é o nível mais básico, focado em ações concretas e burocráticas. Envolve a coleta de documentos, a compra de bilhetes aéreos e a reserva de acomodações. Aqui, o sucesso é medido pela conclusão de uma lista de verificação (check-list).

Nível Gerencial (Otimização de Recursos):
Nesta etapa, o foco deixa de ser a tarefa isolada e passa a ser a logística integrada. Analisamos a relação custo-benefício, a viabilidade de conexões entre transportes e a gestão do tempo. É o momento em que se projeta como os recursos (tempo e dinheiro) serão distribuídos para maximizar a eficiência da jornada.

Nível Cognitivo (Impacto e Experiência):
A abstração mais alta foca no propósito da viagem. Trata-se da exposição ao desconhecido e da adaptação a novas normas sociais e culturais. Neste nível, a viagem é vista como um processo de expansão intelectual, onde o indivíduo processa informações externas para reconfigurar sua própria visão de mundo.

2. Lógica Estrutural (Pseudocódigo em Python
O código abaixo representa a lógica de decisão necessária para viabilizar o projeto:

def planejar_viagem_internacional(destino, orçamento_disponivel):
    # Inicialização de variáveis de controle
    documentos_ok = verificar_requisitos_legais()
    custo_estimado = calcular_logistica(destino)
    
    # Validação de viabilidade (Nível Operacional e Gerencial)
    if documentos_ok and custo_estimado <= orçamento_disponivel:
        print("Projeto viável. Iniciando reservas.")
        realizar_transacoes()
    else:
        print("Projeto inviável. Ajustar destino ou orçamento.")
        return False

    # Fase de Execução e Adaptação (Nível Cognitivo)
    em_transito = True
    while em_transito:
        executar_itinerario()
        if detectar_imprevisto():
            recalcular_rota() # Resiliência sistêmica
        
        if data_retorno == True:
            em_transito = False
            
    return "Viagem concluída: Integração cultural realizada."





    
3. O fluxo a seguir detalha o caminho crítico do planejamento à conclusão:

        A[Início: Ideia da Viagem] --> B{Tem Orçamento?}
    
        B -- Não --> C[Fase de Economia]
        C --> B
    
        B -- Sim --> D[Verificar Documentação]
    
        D --> E{Passaporte/Visto OK?}
        E -- Não --> F[Processo de Emissão]
        F --> D
    
        E -- Sim --> G[Reservar Passagem e Hotel]
    
       G --> H[Execução da Viagem]
    
       H --> I{Surgiu Imprevisto?}
       I -- Sim --> J[Ajustar Roteiro]
       J --> H
    
       I -- Não --> K[Fim: Retorno e Experiência]
