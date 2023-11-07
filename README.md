# Обучение с подкреплением, ВМК МГУ, осень 2023

В отличие от классического машинного обучения, в обучении с подкреплением алгоритму на вход не поступает обучающая выборка. Вместо этого, обучение проводится "методом проб и ошибок": агент должен сам собрать данные в ходе взаимодействия с окружающим миром (средой) и на основе собранного опыта научиться максимизировать получаемый отклик - подкрепление, или награду. Курс направлен на изучение алгоритмов последних лет, показывающих state-of-the-art результаты во многих задачах дискретного и непрерывного управления за счёт совмещения классической теории с парадигмой глубинного обучения.

Проводится для магистров групп 617, 522, 622.

**Преподаватели**: Кропотов Дмитрий, Темирчев Павел, Синильщиков Илья, Медведев Алексей, Медведев Дмитрий, Ипполитов Владимир, Сюй Миньчуань

**Расписание**: курс проводится в смешанном онлайн/офлайн режиме по пятницам, лекция в 14-35, семинар в 16-20 в ауд. 526б.

**Канал в Telegram**: [ссылка](https://t.me/+vZ-2d2ov5Pc5YTcy)

**Видеозаписи занятий**: [текущий год](https://www.youtube.com/playlist?list=PLVF5PzSHILHQefZ-fAbapNqi7AMQoqL-D), [прошлый год](https://www.youtube.com/playlist?list=PLVF5PzSHILHShpQTIiYiR-kGEHLfYx9Qo)

## Критерии оценки

В курсе предусмотрено шесть лабораторных работ в формате ноутбуков и письменный экзамен. Итоговая оценка по курсу в 10-балльной шкале рассчитывается по формуле:

Итоговая оценка = Округл.вверх (0.3 * Экз + 0.7 * Лаб)

Оценке 5 в пятибалльной шкале соответствует оценка 8 и выше, оценке 4 - оценка [6, 8), оценке 3 - промежуток [4, 6). Помимо баллов необходимо также выполнить следующие условия:

| Итог | Необходимые условия |
| :---: | :---: | 
| 5	  | сдано не менее 5 заданий, оценка за экзамен >= 6
| 4	  | сдано не менее 4 заданий, оценка за экзамен >= 4
| 3   |	сдано не менее 3 заданий, оценка за экзамен >= 4

## Домашние задания
Максимальный балл за лабораторные - 100 баллов; итоговая оценка за лабораторные получается делением на десять. За некоторые задания можно будет получить бонусные баллы, о чем будет объявляться при выдаче задания.

Сдавать лабораторные можно в течение недели после мягкого дедлайна (работы сданные в этот период облагаются штрафом: см. таблицу ниже). Лабораторные, сданные позже недели после мягкого дедлайна, не приносят баллов, но учитываются в необходимых условиях для конкретной оценки (см. выше).

| Лабораторная	| Ориентировочная дата выдачи<br>(может быть изменена!) | Срок | Баллы | Штраф<br> за день опоздания |
| :---: | :---: | :---: | :---: | :---: |
| CEM	| 9 сентября	| 1 неделя | 10 |	-0.3
| PI, VI | 19 сентября | 1 неделя	| 10 | -0.3
| DQN	| 9 октября	| 2 недели | 20	| -0.6
| A2C	| 6 ноября | 2 недели	| 20 | -0.6
| PPO	| 21 ноября	| 2 недели | 20	| -0.6
| MCTS | 6 декабря | 2 недели	| 20 | -0.6

## Расписание занятий
| Дата | Формат | Занятие	| Материалы	| Дополнительные материалы	| 
| :---: | :---: | --- | --- | --- |
| Лекция<br>8 сентября | Онлайн | Введение в курс. Кросс-энтропийный метод (CEM).	| [CEM for optimization](https://people.smp.uq.edu.au/DirkKroese/ps/CEopt.pdf)<br> [Tetris with CEM](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.81.6579&rep=rep1&type=pdf) | [OpenAI ES](https://openai.com/blog/evolution-strategies/)<br> [Обзор эволюционных стратегий](https://lilianweng.github.io/lil-log/2019/09/05/evolution-strategies.html)<br> [WANN](https://arxiv.org/pdf/1906.04358.pdf) |
| Семинар<br>8 сентября | Онлайн | Библиотека OpenAI gym. Реализация табличного кросс-энтропийного метода. |   |   |			
| Лекция<br>15 сентября | Онлайн | Динамическое программирование. Value Iteration, Policy Iteration. | [Sutton, Barto, ch.3-4](https://drive.google.com/file/d/1Z4W_-0IaMNpZnhnMkqcDVM_EA79GFJo-/view) | [A (Long) Peek into Reinforcement Learning](https://lilianweng.github.io/lil-log/2018/02/19/a-long-peek-into-reinforcement-learning.html) |
Лекция
30 сентября

Табличные методы. TD-обучение.	
Слайды занятия
Sutton, Barto, ch.5-6
Визуализация TD-обучения (distill)
Семинар
30 сентября

Табличное Q-обучение.			
Лекция
7 октября

Deep Q-Network (DQN) и его модификации.	
Слайды занятия
DQN
Double DQN
Prioritized Experience Replay
Noisy Networks
Dueling DQN
R2D2
Agent57
Семирнар
7 октября

Модификации DQN.			
Лекция
14 октября

Distributional RL. Quantile Regression DQN (QR-DQN).	
Categorical DQN
QR-DQN
Implicit Quantile Networks (IQN)
Rainbow DQN
Семинар
14 октября

Distributional RL - продолжение.			
Лекция
21 октября

Многорукие бандиты.	
полезный ресурс по бандитам
Семинар
21 октября

Внутренняя мотивация для исследования среды.	
Слайды занятия
Sutton, Barto, ch.2
Random Network Distillation (RND)
Intrinsic Curiosity Module (ICM)
Обзор модулей внутренней мотивации
Variational Information Maximizing Exploration (VIME)
Never Give Up (NGU)
Лекция
28 октября

Policy gradient подход. Advantage Actor-Critic (A2C).	
Sutton, Barto, ch.13
A2C
Обзор Policy Gradient алгоритмов
Комикс про A2C
Семинар
28 октября

REINFORCE.			
Лекция
11 ноября

Trust-Region Policy Optimization (TRPO).	
TRPO
Лекция
18 ноября

Proximal Policy Optimization (PPO).	
Слайды занятия
PPO
Implementation matters in RL
Семинар
18 ноября

Generalized Advantage Estimation (GAE).	
GAE
Sutton, Barto, ch.12
Лекция
25 ноября

Непрерывное управление.	
Deep Deterministic Policy Gradient (DDPG)
Twin-Delayed DDPG (TD3)
Soft Actor-Critic (SAC)
Truncated Quantile Critics (TQC)
Семинар
25 ноября

Soft Actor Critic. Управление, как вероятностный вывод.	
RL as probabilistic inference
Лекция
2 декабря

Имитационное обучение.			
Семинар
2 декабря

Обратное обучение с подкреплением.	
Guided Cost Learning
Generative Adversarial Imitation Learning (GAIL)
Лекция
9 декабря

Monte Carlo Tree Search.			
Семинар
9 декабря

AlphaZero, MuZero.	
AlphaZero
MuZero
AlphaZero in one picture
Лекция
16 декабря

Linear Quadratic Regulator (LQR). Model-based RL.	
Презентация по MCTS и LQR
Презентация по Model-based RL
World Models
Семинар
16 декабря

Dreamer	
Dreamer v1
Dreamer v2


