class Quality ControlSystem:
def init_(self):
self.products = []
self.defects = []
def add_product(self, product_id, product_name):
self.products.append({"product_id": product_id, "product_name": product_name})
def add_defect(self, product_id, defect_description):
self.defects.append({"product_id": product_id, "defect_description": defect_description})
def generate_report(self):
report = "Quality Control Report:\n"
for defect in self.defects:
report += f"Product ID:
{defect['product_id']}, Defect: {defect['defect_description']}\l
return report
qc_system QualityControlSystem()
qc_system.add_product("P001", "Product A")
qc_system.add_product("P002", "Product B")
qc_system.add_defect("P001", "Defect in material")
qc_system.add_defect("P001", "Defect in assembly")
qc_system.add_defect("P002", "Defect in packaging")
report qc_system.generate_report()
print(report)
