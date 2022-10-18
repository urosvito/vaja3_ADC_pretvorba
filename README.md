# Vaja3-ADC-trigger-timer-conversion-STM32F4


Cilj naloge: S pomočjo programskega okolja STM32CubeIDE in HAL knjižnicami sprogramirajte mikroprocesor tako, da bo izvajal ADC pretvorbe sprožene s časovnimi prekinitvami (interrupt).

ODGOVORI NA VPRAŠANJA:
Uporabljena razvojna plošča je STM32F401C-DISCO
B) Izbran pin je PA1 na plošči je to tudi PA1.
E) Poleg pina se izpiše ADC1_IN1
H) LED je že aktivirana.
I) Ko spremenimo APB1 Timer na 16 MHz se spremenijo tudi APB1 peripheral clocks, APB2 peripheral clocks...
L) Če želimo frekvenco nastaviti na 1 kHz moramo v polje Prescaler zapisati 16 000 zaradi drugačnih enot.
F) Za spreminjanje stanje LED je uporabljena komanda HAL_GPIO_TogglePin(GPIOD, GPIO_PIN_12);



KOMENTAR:
Pri točki e je sampling time 28;
Namesto TIM 1 moramao izbrati TIM 3 saj TIM 1 nima opcije Timer trigger out event;
Koda ne dela na STM32F401C-DISCO.
