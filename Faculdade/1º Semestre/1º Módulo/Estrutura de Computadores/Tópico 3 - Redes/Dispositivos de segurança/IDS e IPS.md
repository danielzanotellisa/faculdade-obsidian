---
tags:
  - Conceitos_de_redes
  - Dispositivos
  - Rede
  - Segurança
---
## IDS
---

Os IDS ([Intrusion Detection System](https://pt.wikipedia.org/wiki/Sistema_de_detec%C3%A7%C3%A3o_de_intrusos)) monitoram passivamente o tráfego na rede, onde uma cópia de tudo oque passa por ela vai para um console de gerenciamento e lá esse fluxo é comparado com assinaturas reconhecidamente mal-intencionadas como um software que verifica a existência de vírus.

## IPS
___

Um IPS ([Intrusion Prevention System](https://www.vmware.com/topics/glossary/content/intrusion-prevention-system.html#:~:text=An%20intrusion%20prevention%20system%20(IPS,it%2C%20when%20it%20does%20occur.))) se baseia numa IDS, porém, a sua grande diferença é que ele faz um monitoramento ATIVO do fluxo de tráfego, ou seja, o tráfego só é autorizado a passar para o lado seguro da rede após ser analisado, caso algo malicioso seja encontrado, será descartado. Todo o tráfego de saída e entrada flui por ele para ser processado.
