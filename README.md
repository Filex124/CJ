# CJ
"HELLO CJ"
  def __init__(self, name, email, password, address, vehicle, vehicle_type, capability, route_range, phone):
    self.name = name
    self.email = email
    self.password = password
    self.address = address
    self.vehicle = vehicle
    self.vehicle_type = vehicle_type
    self.capability = capability
    self.route_range = route_range
    self.phone = phone
    self.bank_info = {}
  
  def register_payment_info(self, bank_name, account_number, routing_number):
    self.bank_info['bank_name'] = bank_name
    self.bank_info['account_number'] = account_number
    self.bank_info['routing_number'] = routing_number
  
  def update_location(self, lat, lng):
    self.lat = lat
    self.lng = lng
  
  def receive_delivery_request(self, customer_info, provider_info):
    self.customer_info = customer_info
    self.provider_info = provider_info
  
  def contact_customer(self, method):
    if method == 'call':
      make_call(self.customer_info['phone'])
    elif method == 'chat':
      send_message(self.customer_info['name'], 'Hello, this is your delivery guy. How can I help you?')

![image](https://user-images.githubusercontent.com/122705793/212502497-48d47e08-999e-46a1-aebd-47eb1d7832f6.png)
