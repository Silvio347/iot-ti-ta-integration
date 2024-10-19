# iot-ti-ta-integration
Devido ao tamanho do projeto, por enquanto está no drive: https://drive.google.com/drive/folders/1R-PCmGsQxgBLUHSn0TjFAI61nTSDnIVb?usp=sharing

⚙️ Projeto de Aprendizado: Integração IoT e Conexão TI e TA ⚙️

Gostaria de compartilhar um projeto que desenvolvi recentemente para aprimorar minhas habilidades em IoT e integração entre TI e TA! Trabalhei na visualização da variação de um sensor de temperatura, simulada com um potenciômetro.

🔌 Resumo:

* O ESP32 captura os dados e envia via MQTT para um broker, que registra no banco de dados sempre que a temperatura ultrapassa limites definidos.
* As aplicações estão encapsuladas em Docker, facilitando a implantação.
* Criei um app em Flutter para visualização e controle local do sistema, com LEDs físicos e virtuais indicando níveis de temperatura.
* Também utilizei o Blynk para oferecer as mesmas funcionalidades do app, com acesso remoto de qualquer lugar.

🔧 Ferramentas Utilizadas:

🐍 FastAPI + PostgreSQL + Pydantic: API para salvar e exibir registros de data, hora e temperatura. A exibição dos registros fica na página WEB que o ESP32 gera, onde também é possível parametrizá-lo.
🦟 Mosquitto: No mesmo script Python onde configurei a API, configurei o broker MQTT para receber os dados enviados pelo ESP32.
🕒 FreeRTOS: Realizei a divisão de tarefas no ESP32, aproveitando seus núcleos para garantir um funcionamento eficiente e organizado do sistema.
🐳 Docker: Encapsulei as aplicações, facilitando a implantação e gerenciamento do ambiente.
🌐 Blynk: Utilizei a plataforma como supervisório, devido à sua escalabilidade, acesso de qualquer lugar e facilidade de uso.
🔄 OTA (Over The Air): Atualização de firmware e parâmetros via página web.
📱 Flutter: Parametrização do ESP32 e monitoramento remoto sincronizado com o Blynk.

Este projeto me proporcionou um aprendizado profundo em conceitos essenciais de TI, TA e IoT. Foi um grande passo na exploração de tecnologias que conectam o mundo físico e digital! 🚀
