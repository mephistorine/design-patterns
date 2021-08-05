# Фабричный метод

## Другие названия

- Виртуальный конструктор
- Factory Method

## Семейство

Порождающий

## Определение

**Фабричный метод** — это порождающий паттерн проектирования, который определяет общий интерфейс для создания объектов в суперклассе, позволяя подклассам изменять тип создаваемых объектов.

```mermaid
classDiagram
	class Creator {
	  + createProduct() Product
	}
	
	Creator --> Product
	
	Creator <|-- ConcreteCreatorA
	
	Creator <|-- ConcreteCreatorB
	
	class Product {
	}
	
	class ConcreteCreatorA {
	  + createProduct() Product
	}
	
	class ConcreteCreatorB {
	  + createProduct() Product
	}
```