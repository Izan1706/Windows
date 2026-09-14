# 🛠️ Windows Update Management Scripts (Disable & Re-enable)

Conjunto de scripts Batch (`.bat` / `.cmd`) diseñados para deshabilitar o reactivar por completo el servicio de Windows Update, las directivas de grupo, el servicio Medic de Windows Update (`WaaSMedicSvc`) y sus tareas programadas asociadas en Windows 10 y Windows 11.

---

## ⚠️ Advertencia de Seguridad Importante

> **¡ATENCIÓN! LEA ANTES DE USAR:**
> * Desactivar Windows Update **no es una práctica recomendada** para uso diario, ya que impide la recepción de parches de seguridad y actualizaciones del sistema, dejando el equipo expuesto a vulnerabilidades.
> * Utilice este script únicamente en entornos de pruebas, laboratorios, servidores aislados o cuando sea estrictamente indispensable pausar/bloquear las actualizaciones.

---

## 📌 Contenido del Repositorio

* **`Desactivar_Windows_Update.bat`**: Detiene y deshabilita los servicios de actualización (`wuauserv`, `bits`, `dosvc`, `usosvc`, `WaaSMedicSvc`), aplica directivas en el Registro para bloquear las actualizaciones automáticas, deshabilita las tareas programadas relacionadas y limpia la cola de descargas (`SoftwareDistribution` / `catroot2`).
* **`Reactivar_Windows_Update.bat`**: Revierte completamente todos los cambios aplicados: restaura la configuración de inicio de los servicios, habilita las tareas programadas, elimina las directivas de bloqueo del Registro, inicia los servicios de nuevo e inicia un escaneo de actualizaciones.

---

## 📋 Requisitos Previos

* **Sistema Operativo:** Windows 10 o Windows 11.
* **Permisos:** Se requieren privilegios de **Administrador** para ejecutar ambos scripts.

---

# 🛠️ Windows Update Management Scripts (Disable & Re-enable)

A set of Batch scripts (`.bat` / `.cmd`) designed to completely disable or re-enable the Windows Update service, Group Policies, the Windows Update Medic Service (`WaaSMedicSvc`), and associated scheduled tasks in Windows 10 and Windows 11.

---

## ⚠️ Important Security Warning

> **ATTENTION! READ BEFORE USING:**
> * Disabling Windows Update **is not a recommended security practice** for daily use, as it prevents the system from receiving security patches and updates, leaving the machine vulnerable.
> * Use these scripts only in testing environments, lab setups, isolated servers, or when strictly necessary to pause/block updates.

---

## 📌 Repository Contents

* **`Desactivar_Windows_Update.bat`**: Stops and disables update services (`wuauserv`, `bits`, `dosvc`, `usosvc`, `WaaSMedicSvc`), applies Registry policies to block automatic updates, disables related scheduled tasks, and clears the download queue (`SoftwareDistribution` / `catroot2`).
* **`Reactivar_Windows_Update.bat`**: Fully reverts all changes: restores service startup configurations, re-enables scheduled tasks, deletes blocking Registry policies, restarts the required services, and triggers an update scan.

---

## 📋 Prerequisites

* **Operating System:** Windows 10 or Windows 11.
* **Privileges:** **Administrator** rights are required to execute both scripts.

---
