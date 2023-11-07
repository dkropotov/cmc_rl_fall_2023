# Обучение с подкреплением, ВМК МГУ, осень 2023

В отличие от классического машинного обучения, в обучении с подкреплением алгоритму на вход не поступает обучающая выборка. Вместо этого, обучение проводится "методом проб и ошибок": агент должен сам собрать данные в ходе взаимодействия с окружающим миром (средой) и на основе собранного опыта научиться максимизировать получаемый отклик - подкрепление, или награду. Курс направлен на изучение алгоритмов последних лет, показывающих state-of-the-art результаты во многих задачах дискретного и непрерывного управления за счёт совмещения классической теории с парадигмой глубинного обучения.

Проводится для магистров групп 617, 522, 622.

**Преподаватели**: Кропотов Дмитрий, Темирчев Павел, Синильщиков Илья, Медведев Алексей, Медведев Дмитрий, Ипполитов Владимир, Сюй Миньчуань

**Расписание**: курс проводится в смешанном онлайн/офлайн режиме по пятницам, лекция в 14-35, семинар в 16-20 в ауд. 526б.

**Зум для онлайн-занятий**: [ссылка](https://us02web.zoom.us/j/86204571845?pwd=WDZBQUU2aVdNTmNkRGZqVU9TWDNHdz09)

**Чат в Telegram для вопросов и обсуждений**: [ссылка](https://t.me/+vZ-2d2ov5Pc5YTcy)

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
| Лекция<br>30 сентября | Офлайн | Табличные методы. TD-обучение.	| [Слайды занятия](http://www.machinelearning.ru/wiki/images/3/34/TD_learning_2021.pdf)<br>[Sutton, Barto, ch.5-6](https://drive.google.com/file/d/1Z4W_-0IaMNpZnhnMkqcDVM_EA79GFJo-/view) | [Визуализация TD-обучения (distill)](https://distill.pub/2019/paths-perspective-on-value-learning/) |
| Семинар<br>30 сентября | Онлайн | Табличное Q-обучение. |  |  |
| Лекция<br>7 октября | Офлайн | Deep Q-Network (DQN) и его модификации. | [Слайды занятия](http://www.machinelearning.ru/wiki/images/3/3c/Deep_Q_learning_2021.pdf)<br>[DQN](https://www.cs.toronto.edu/~vmnih/docs/dqn.pdf)<br>[Double DQN](https://arxiv.org/pdf/1509.06461.pdf)<br>[Prioritized Experience Replay](https://arxiv.org/pdf/1511.05952.pdf)<br>[Noisy Networks](https://arxiv.org/abs/1706.10295)<br>[Dueling DQN](https://arxiv.org/abs/1511.06581) | [R2D2](https://openreview.net/pdf?id=r1lyTjAqYX)<br>[Agent57](https://arxiv.org/abs/2003.13350) |
| Семинар<br>7 октября | Онлайн | Модификации DQN. |  |  |
| Лекция<br>14 октября | Офлайн | Distributional RL. Quantile Regression DQN (QR-DQN). | [Categorical DQN](https://arxiv.org/pdf/1707.06887.pdf)<br>[QR-DQN](https://arxiv.org/pdf/1710.10044.pdf) | [Implicit Quantile Networks (IQN)](https://arxiv.org/pdf/1806.06923.pdf)<br>[Rainbow DQN](https://arxiv.org/pdf/1710.02298.pdf) |
| Семинар<br>14 октября | Офлайн | Distributional RL - продолжение.	|  |  |
| Лекция<br>21 октября | Офлайн | Многорукие бандиты.	| [полезный ресурс по бандитам](https://banditalgs.com/) |   |
| Семинар<br>21 октября | Офлайн | Внутренняя мотивация для исследования среды.	| [Слайды занятия](http://www.machinelearning.ru/wiki/images/f/fa/Exploration-vs-exploitation.pdf)<br>[Sutton, Barto, ch.2](https://drive.google.com/file/d/1Z4W_-0IaMNpZnhnMkqcDVM_EA79GFJo-/view)<br>[Random Network Distillation (RND)](https://arxiv.org/abs/1810.12894)<br>[Intrinsic Curiosity Module (ICM)](https://arxiv.org/abs/1705.05363) | [Обзор модулей внутренней мотивации](https://lilianweng.github.io/lil-log/2020/06/07/exploration-strategies-in-deep-reinforcement-learning.html)<br>[Variational Information Maximizing Exploration (VIME)](https://arxiv.org/abs/1605.09674)<br>[Never Give Up (NGU)](https://arxiv.org/abs/2002.06038) |
| Лекция<br>28 октября | Офлайн | Policy gradient подход. Advantage Actor-Critic (A2C).	| Sutton, Barto, ch.13<br>A2C | Обзор Policy Gradient алгоритмов<br>Комикс про A2C |
| Семинар<br>28 октября | Офлайн | REINFORCE.	|  |  |
| Лекция<br>11 ноября | Онлайн | Trust-Region Policy Optimization (TRPO).	| TRPO |  |
| Лекция<br>18 ноября | Офлайн | Proximal Policy Optimization (PPO). | Слайды занятия<br>PPO | Implementation matters in RL |
| Семинар<br>18 ноября | Офлайн | Generalized Advantage Estimation (GAE).	| GAE | Sutton, Barto, ch.12 |
| Лекция<br>25 ноября | Офлайн | Непрерывное управление. | Deep Deterministic Policy Gradient (DDPG)<br>Twin-Delayed DDPG (TD3)<br>Soft Actor-Critic (SAC) | Truncated Quantile Critics (TQC) |
| Семинар<br>25 ноября | Офлайн | Soft Actor Critic. Управление, как вероятностный вывод.	| RL as probabilistic inference |   |
| Лекция<br> 2 декабря | Офлайн | Имитационное обучение.	|  |
| Семинар<br>2 декабря | Офлайн | Обратное обучение с подкреплением.	| Guided Cost Learning<br>Generative Adversarial Imitation Learning (GAIL) |  |
| Лекция<br>9 декабря | Офлайн | Monte Carlo Tree Search.		|  |  |
| Семинар<br>9 декабря | Офлайн | AlphaZero, MuZero.	| AlphaZero<br>MuZero | AlphaZero in one picture |
| Лекция<br>16 декабря | Онлайн | Linear Quadratic Regulator (LQR). Model-based RL.	| Презентация по MCTS и LQR<br>Презентация по Model-based RL | World Models |
| Семинар<br> 16 декабря | Онлайн | Dreamer	| Dreamer v1<br>Dreamer v2 |  |

## Материалы
[Полунеофициальный конспект](https://github.com/FortsAndMills/RL-Theory-book/blob/main/RL_Theory_Book.pdf)

[Курс Practical RL (ШАД)](https://github.com/yandexdataschool/Practical_RL)

[Курс Deep Reinforcement Learning (CS 285), UC Berkeley](https://www.youtube.com/playlist?list=PLkFD6_40KJIxJMR-j5A1mkxK26gh_qg37)
