# Automatizador--de-tabelas-usando-Pyautogui
Uma automatização de processos utilizando Pyautogui para preencher listas e tabelas de forma ágil.

#link para testes: https://dlp.hashtagtreinamentos.com/python/intensivao/login

O 1PyAUtoGui.py é um automação GUI baseada em coordenadas que usa pyautogui para controlar o Chrome e pandas para ler uma planilha CSV (produtos.csv). O script navega até uma URL de login, abre o navegador via busca do Windows, escreve o link, e fornece credenciais (PaToGato123) em campos pré-posicionados. Em seguida carrega produtos.csv e, para cada linha, localiza campos do formulário pela posição do cursor (clique em coordenadas fixas) e escreve os valores das colunas: codigo, marca, tipo, categoria, preco_unitario, custo e obs. Após cada registro, envia o formulário (enter) e faz um scroll para processar o próximo item.

Pontos importantes: o script usa coordenadas estáticas e delays fixos (time.sleep, pyautogui.PAUSE), o que o torna frágil a mudanças de layout, resolução ou de desempenho da máquina. Ele tem credenciais em texto plano e desativa parcialmente o failsafe, com alguns riscos de segurança e confiabilidade. Não há tratamento de erros, validação de dados nem retorno estruturado, a saída é apenas a ação no navegador.

OBS: Utilizar o codespace para testar o código no próprio navegador.
