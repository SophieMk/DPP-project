# DPP-project: Engine condition monitoring

## Задание

### Предсказать performance значения для каждого полетного цикла.

В input данных 53 параметра (50 уникальных + engine_id, flight_datetime, flight_phase).

В output данных 33 параметра (30 уникальных + engine_id, flight_datetime, flight_phase). 

P.S. Обратите внимание на четвертую главу методики оценки состояния двигателей.

### Предсказать необходимое ТО для двигателей

В соотвествии с правилами, описанными в шестой главе методики оценки состояния двигателей, предскажите дефекты и соотвествующее ТО для каждого двигателя.

P. S. Совет: Мерджить X и y можно по 3 полям: [engine_id", "flight_datetime", "flight_phase"]. Например: pd.merge(X, y, on=["engine_id", "flight_datetime", "flight_phase"])
