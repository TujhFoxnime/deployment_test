* Deployment:
 Запросы (requests) соответствуют нормальной нагрузке, лимиты (limits) обеспечивают возможность использования большего количества ресурсов при инициализации.
 podAntiAffinity обеспечит распределение подов по различным нодам для повышения отказоустойчивости.

* HorizontalPodAutoscaler:
 Минимальное количество реплик - 2, чтобы ночью было минимальное потребление ресурсов.
 Максимальное количество реплик - 8, чтобы обеспечить покрытие пиков.

* PodDisruptionBudget:
 Обеспечивает, что минимум 3 пода всегда будут работать, что гарантирует отказоустойчивость.
