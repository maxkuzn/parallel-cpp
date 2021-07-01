## Multiple Producer Single Consumer Queue

В этой задаче необходимо реализовать lock-free stack. Multiple producer single consumer означает, что множество потоков могут добавлять элементы в стек, но только один поток может их извлекать.  

Каждый элемент хранится в структуре Node, также в Node хранится указатель на следующий элемент. Таким образом, образуется односвязный список. Сам стек в свою очередь хранит в себе указатель на голову списка.

---

В этой задаче также нужно использовать CAS операции. Запрещается использовать блокировки.