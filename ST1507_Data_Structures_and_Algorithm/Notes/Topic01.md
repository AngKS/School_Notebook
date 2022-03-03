
# Topic 01: Introduction to Data Structures & Algorithms(AI)

| Topics                                            | [Link]() |
| :------------------------------------------------ | :------- |
| Data, Structures & Algorithm.                     | [Link]() |
| Abstract Data Types, and information hiding (OOP) | [Link]() |
| Big O-Notation                                    | [Link]() |


### Data and related terms

| Word        | Meaning                                                                                             | Example                                                                                                            |
| :---------- | :-------------------------------------------------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------------- |
| Data[^1]    | A certain sequence of symbols that is open for interpretation                                       |                                                                                                                    |
| Information | Data that has been interpreted in the context of metadata [^2]                                      | "Our ship is in distress, please help"                                                                             |
| Knowledge   | Theoretical/Practical understanding of a subject                                                    | "The captain and crew will be able to navigate our ship through these stormy weathers"                             |
| Wisdom      | The ability to think and act using knowledge, experience, understanding, common sense and insights. | "As the captain of the ship, I have decided we will delay our journey for a day due to the bad weather forecasts." |

## Structures (Generic)

> A structure refers to the organization of a collection of related components that forms a whole, so it can support a certain function.

For instance, a man-made structure such as a building, is a collection of related parts, that are put together (organised) as to support a load bearing function (a brige, for instance).

## Structures (Computer Science)

> Data Structures describes a collection of data values, the relationships between these data values, and the functions that can be applied to these data values.

A data structure would need to support efficiency (in terms of storage and access) and flexibility.

## Arrays vs Linked Lists

### Array Data Structures

> An Array is a Data Structure that stores data in a continuous block of computer memory

| Address  | Value |
| :------- | :---- |
| 00:FF:01 | 97    |
| 00:FF:02 | 98    |
| 00:FF:03 | 99    |
| 00:FF:04 | 100   |

To ‘squeeze’ in an extra value between the address ```00:FF:02``` and ```00:FF:03``` we would need to shift the values by one memory address.

<table>
    <tr>
        <th>Before Shift</th>
        <th>After Shift</th>
    <tr>
        <td>
            | Address  | Value |
            | :------- | :---- |
            | 00:FF:01 | 97    |
            | 00:FF:02 | 98    |
            | 00:FF:03 | 99    |
            | 00:FF:04 | 100   |
        </td>
        <td>
            | Address  | Value      |
            | :------- | :--------- |
            | 00:FF:01 | 97         |
            | 00:FF:02 | 98         |
            | 00:FF:03 | {newValue} |
            | 00:FF:04 | 99         |
            | 00:FF:05 | 100        |
        </td>
    </tr>

</table>


| Advantages                  | Disadvantages                       |
| :-------------------------- | :---------------------------------- |
| - Allow for Random Copy     | - Have Fixed Size                   |
| - Easy to Copy              | - Difficult to Expand with new Data |
| - Uses less Computer Memory |                                     |

Arrays would typically store Homogenous Data (eg. the same kinds of data, like a series of integers, characters, floats, whereby all units of data have the same data size.)


### Linked List Data Structures

> A Linked List Data Structure, unlike arrays, does not stores data in one continuous piece of computer memory. However it breaks data down into **Nodes**[^3].








[^1]: **Data** is a sequence of symbols that can be translated into information through an act of interpretation (or an act of analyses).

[^2]: **Metadata** is the context that allows us to translate data into information.

[^3]: Nodes are units of storage that store data, as well as a reference to a memory address from another node. (That other node could be located anywhere else in the computer memory.) 


