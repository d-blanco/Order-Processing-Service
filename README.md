# Order Processing Service

The Order Processing Service handles customer orders for the business. It allows users to create, view, and manage orders. This service is critical to operations, as errors may directly impact revenue and customer experience.

## Endpoints

### GET /orders
Returns a list of all orders.

- **Description**: Retrieves all existing orders in the system.
- **Use Case**: Used by support teams and dashboards to view current orders.

---

### GET /orders/{id}
Returns a specific order by ID.

- **Description**: Retrieves details for a single order.
- **Use Case**: Used to investigate or track a specific customer order.

---

### POST /orders
Creates a new order.

- **Description**: Accepts order data and creates a new order record.
- **Use Case**: Used by applications or users to submit new customer orders.

---

### PUT /orders/{id}
Updates an existing order.

- **Description**: Modifies an existing order's details.
- **Use Case**: Used to correct or update order information.

---

### DELETE /orders/{id}
Deletes an order.

- **Description**: Removes an order from the system.
- **Use Case**: Used for cleanup or handling invalid/test orders.

---

## Notes

- All changes to this service must follow the defined promotion process across environments (dev → QA → prod).
- Proper validation and testing are required before promoting changes to production.
